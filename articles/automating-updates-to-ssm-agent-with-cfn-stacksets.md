---
title: "AWSでSSMエージェントの自動更新をCloudFormationのスタックセット(StackSets)で複数リージョンx複数アカウントに適用する"
emoji: "🤖"
type: "tech" # tech: 技術記事 / idea: アイデア
topics: ["AWS", "systemsmanager", "cloudformation", "organizations"]
published: false
---

# はじめに

:::message
ドキュメントに明記されたものではないため、現時点での動作確認結果であり、UIや仕様が変わらないことは保証できない点はご了承ください💡
::

AWSアカウントの管理をしている中で、ふとこんなことを思いました。
「SSMエージェントの自動更新の設定をしたいが、公式ドキュメントで推奨されているマネジメントコンソールからの設定は各アカウントのリージョンごとでしかできないので、マルチアカウントで複数リージョンを一気に設定したい場合どうしよう？」

そこで調べてみてもピンポイントなドキュメントが見つけられなかったので、自分なりにやってみた方法とその中で気になった点をまとめました。実はやりたかったんだよなーという方がいた場合の参考になれば(,,•﹏•,,)

# 要約・結論
- マネジメントコンソールの [Systems Manager] => [フリートマネージャー] で [SSMエージェントの自動更新] を適用した内容は、CloudFormationのテンプレートファイルに[`"Type" : "AWS::SSM::Association"`](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-ssm-association.html)で用意することができた
  - // TODO 作成したテンプレートファイルはこちら
- CloudFormationのStackSetsで複数リージョンx複数アカウントに作成したテンプレートファイルを適用することができた
- // TODO 公式ドキュメントで推奨されているマネジメントコンソールからの適用ではないが、ステートマネージャーの関連付けの名前(Assosiation name)を`SystemAssociationForSsmAgentUpdate`にするとマネジメントコンソール上も適用済みになっていることが確認できた

# SSMエージェントの自動更新について
AWS Systems Managerを利用するためにはSSMエージェントをサーバーにインストールするが、定期的に最新版に更新されているのでインストール後もバージョンアップが推奨される。(// TODO アプリの場所)しかしサーバーの台数が多いと作業も手間になるし、ミスも増えるのでAWSでは自動更新する方法が提供されている。

https://docs.aws.amazon.com/ja_jp/systems-manager/latest/userguide/ssm-agent-automatic-updates.html

方法はいくつか記載されているが、推奨されているのは「マネジメントコンソールの [Systems Manager] => [フリートマネージャー] から設定する」方法である。

実際に試してみると、適用前は以下の表示がされており
// TODO 画像

適用すると以下のような状態になる
// TODO 画像

しかし推奨されているこの方法は、操作しているアカウントでリージョンごとにマネジメントコントロール上で操作する必要があるので複数リージョンでも設定したい場合少し面倒である…
またマルチアカウント構成の場合各アカウントで個別にリージョンごとに設定してもらうのはあまり良い方法ではない…
そこでこの設定がCloudFormationのテンプレートファイルで用意できれば、StackSetsを利用して複数リージョンやマルチアカウントに一度の作業で適用できそう！だけどこの操作をすると何が設定されているの？

# 公式ドキュメントで推奨されているマネジメントコンソールの [Systems Manager] => [フリートマネージャー] からの設定について
マネジメントコンソールの [フリートマネージャー] から設定した場合、実際はSystems Managerの [ステートマネージャー] という機能に設定がされており、マネジメントコンソールで以下のように確認できる。
// TODO 画像

ステートマネージャーの細かい説明は今回はしないが、関連付け(Assosiations)という自動で実行するSSMドキュメントと対象のサーバーを紐付けた一連の設定が作成される。
つまり今回作成されたこの関連付け(Assosiations)をCloudFormationのテンプレートファイルで用意できればOKである👌

# 作成したCloudFormationのテンプレートファイル
マネジメントコンソールの [フリートマネージャー] から設定した場合に作成されたステートマネージャー(State Manager)内の関連付け(Assosiations)の内容と照らし合わせて作成したテンプレートファイルは以下である。

```yaml:
AWSTemplateFormatVersion: 2010-09-09
Resources:
  SsmAgentAutoUpdateToAllInstances:
    Type: AWS::SSM::Association
    Properties:
      AssociationName: SystemAssociationForSsmAgentUpdate
      MaxConcurrency: 50
      MaxErrors: 10%
      Name: AWS-UpdateSSMAgent
      ScheduleExpression: rate(14 days)
      Targets:
        - Key: InstanceIds
          Values:
          - "*"
      WaitForSuccessTimeoutSeconds: 300
```

一番重要なところは`AssociationName`を`SystemAssociationForSsmAgentUpdate`にしておくことである。フリートマネージャーのマネジメントコンソールで設定する場合は"SystemAssociationForSsmAgentUpdate"という名前で作成される。この名前で作成するとフリートマネージャーのマネジメントコンソール上でも設定済み状態として認識されるようである。

`MaxConcurrency`, `MaxErrors`, `ScheduleExpression`はフリートマネージャーのマネジメントコンソールで設定した場合の値にしているが、要件によって変更して良い部分である。
`WaitForSuccessTimeoutSeconds`はCloudFormationからの適用の場合に関係する値なので、自由に変更して良い。

# CloudFormationのStackSetsで適用しよう！
先ほど作成したテンプレートファイルがあればCloudFormationのStackSetsで複数リージョンや複数アカウントに一気に適用できる！
StackSetsを利用する場合は2パターンあり、事前にロールの設定やOrganizationsの信頼関係などが必要になるので注意
// TODO StackSetsについて簡単に、ロールが事前に必要なので注意など
// TODO Organizationsを利用していれば、組織やOUに参加したら自動で適用してくれる点などついて簡単に


# どうでも良いけど気になったので試してみたシリーズ
## で、CloudFormationで適用した場合はフリートマネージャーのマネジメントコンソールはどうなるの？

## すでにフリートマネージャーのマネジメントコンソールで設定していたところに対して、CloufFormationから適用させてしまったら？
同じ名前でIDが違うものができるだけなのでCloufFormatonでの操作はエラーにならない

## `AssociationName`を`SystemAssociationForSsmAgentUpdate`ではないもので作成したらどうなるの？

## ステートマネージャーで`AssociationName`を`SystemAssociationForSsmAgentUpdate`を作ったらどうなるの？

## `AssociationName`を`SystemAssociationForSsmAgentUpdate`で紐付けるドキュメントを`AWS-UpdateSSMAgent`以外にするとどうなるの？



# おわりに
StackSetsは他にもマルチアカウント構成での必須設定などに使われるので、すでに適用している場合はそのテンプレートファイルの一部に組み込むこと
