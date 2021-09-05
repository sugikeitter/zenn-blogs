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

そこで調べても意外とピンポイントなドキュメントが見つからなかったので、自分でやってみた方法と、やりながら気になった点をまとめました。実はやりたかったんだよなーという方がいた場合の参考になれば(,,•﹏•,,)

# 要約・結論
- マネジメントコンソールの [Systems Manager] => [フリートマネージャー] から設定できるSSMエージェントの自動更新内容をCloudFormationのテンプレートファイルに[`"Type" : "AWS::SSM::Association"`](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-ssm-association.html)で用意し、CloudFormationのStackSetsで複数リージョンx複数アカウントに適用することができた
- 公式ドキュメントで推奨されているマネコンからの適用ではないので、適用後にマネコンがどのように変わるかや、内部的な動きでわかったことをまとめた

# SSMエージェントの自動更新について
SSMエージェントとはAWS Systems Managerを利用するサーバーにインストールさせる

https://docs.aws.amazon.com/ja_jp/systems-manager/latest/userguide/ssm-agent-automatic-updates.html

# 公式ドキュメントで推奨されているマネジメントコンソールの [Systems Manager] => [フリートマネージャー] からからの設定について
実際はステートマネージャーに設定がされている
// TODO もう少し補足

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

一番のポイントは`AssociationName`を`SystemAssociationForSsmAgentUpdate`にしておくことである。フリートマネージャーのマネジメントコンソールで設定する場合は"SystemAssociationForSsmAgentUpdate"という名前で作成される。この名前で作成するとフリートマネージャーのマネジメントコンソール上でも設定済み状態として認識されるようである。

`MaxConcurrency`, `MaxErrors`, `ScheduleExpression`はフリートマネージャーのマネジメントコンソールで設定した場合の値にしているが、要件によって変更して良い部分である。
`WaitForSuccessTimeoutSeconds`はCloudFormationからの適用の場合に関係する値なので、自由に変更して良い。

# CloudFormationのStackSetsで適用しよう！
先ほど作成したテンプレートファイルがあればCloudFormationでリージョンごとに設定できる、けど今回やりたかったのは複数リージョンや複数アカウントに一気に適用したい
そこでStackSetsを利用

// TODO StackSetsについて簡単に、ロールが事前に必要なので注意など
// TODO Organizationsを利用していれば、組織やOUに参加したら自動で適用してくれる点などついて簡単に


# どうでも良いけど気になったので試してみたシリーズ
## で、フリートマネージャーのマネジメントコンソールはどうなるの？

## すでにフリートマネージャーのマネジメントコンソールで設定していたところに対して、CloufFormationから適用させてしまったら？
同じ名前でIDが違うものができるだけなのでCloufFormatonでの操作はエラーにならない

## `AssociationName`を`SystemAssociationForSsmAgentUpdate`ではないもので作成したらどうなるの？

## ステートマネージャーで`AssociationName`を`SystemAssociationForSsmAgentUpdate`を作ったらどうなるの？



# おわりに
StackSetsは他にもマルチアカウント構成での必須設定などに使われるので、すでに適用している場合はそのテンプレートファイルの一部に組み込むこと