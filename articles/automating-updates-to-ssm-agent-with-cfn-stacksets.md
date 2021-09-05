---
title: "AWSでSSMエージェントの自動更新をCloudFormationのスタックセット(StackSets)で複数のリージョンやアカウントに適用"
emoji: "🤖"
type: "tech" # tech: 技術記事 / idea: アイデア
topics: ["AWS", "systemsmanager", "cloudformation", "organizations"]
published: false
---

# はじめに

:::message
ドキュメントに明記されたものではないため、現時点での動作確認結果であり、UIや仕様が変わらないことは保証できない点はご了承ください💡
:::

AWSアカウントの管理をしている中で、ふとこんなことを思いました。
「SSMエージェントの自動更新の設定をしたいが、公式ドキュメントで推奨されているマネジメントコンソールからの設定は各アカウントのリージョンごとでしかできないので、マルチアカウントで複数リージョンを一気に設定したい場合どうしよう？」

そこで調べてみてもピンポイントなドキュメントが見つけられなかったので、自分なりにやってみた方法とその中で気になった点をまとめました。実はやりたかったんだよなーという方がいた場合の参考になれば(,,•﹏•,,)

# 要約・結論
- マネジメントコンソールの [Systems Manager] => [フリートマネージャー] で [SSMエージェントの自動更新] を適用する内容は、CloudFormationのテンプレートファイルに[`AWS::SSM::Association`という`Type`](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-ssm-association.html)で設定できる
  - 作成したテンプレートファイルは[こちら](automating-updates-to-ssm-agent-with-cfn-stacksets#作成したCloudFormationのテンプレートファイル)
- つまりこのテンプレートファイルを利用してCloudFormationのStackSetsで複数リージョンや複数アカウントに一度の手順でSSMエージェントの自動更新を適用可能
- どんなやり方であっても、Systems Managerのステートマネージャーに`SystemAssociationForSsmAgentUpdate`という名前の関連付け(Assosiation)を作成すると、フリートマネージャーのマネジメントコンソール上ではSSMエージェントの自動更新が適用されたという状態になる

# SSMエージェントの自動更新について
AWS Systems Managerを利用するためにはSSMエージェントをサーバーにインストールするが、定期的に最新版に更新されている。
https://github.com/aws/amazon-ssm-agent

そのためインストール後もバージョンアップが推奨されるが、AWSでは自動更新する方法が提供されている🙌
https://docs.aws.amazon.com/ja_jp/systems-manager/latest/userguide/ssm-agent-automatic-updates.html

方法はいくつか記載されているが、2021/09/06現在で推奨されているのは「マネジメントコンソールの [Systems Manager] => [フリートマネージャー] から [SSMエージェントの自動更新] ボタンを押して設定する」方法である。

## マネジメントコンソールのフリートマネージャーから「自動更新」適用前の状態
適用前は「SSMエージェントの自動更新」ボタンが表示されている状態になる↓
![](/images/automating-updates-to-ssm-agent-with-cfn-stacksets/fleet-manager-settings-console-before-automating-updates-to-ssm-agent.png)

## マネジメントコンソールのフリートマネージャーから「自動更新」適用後の状態
適用すると「エージェントの自動更新」の詳細が表示された状態になる↓
![](/images/automating-updates-to-ssm-agent-with-cfn-stacksets/fleet-manager-settings-console-after-automating-updates-to-ssm-agent.png)

しかし推奨されているこの方法は、操作しているアカウントでリージョンごとにマネジメントコントロール上で操作する必要があるので複数リージョンでも設定したい場合少し面倒である…
またマルチアカウント構成の場合、各アカウントで個別にリージョンごとに設定してもらうのは微妙…
そこでこの設定がCloudFormationのテンプレートファイルで用意できれば、StackSetsを利用して複数リージョンやマルチアカウントに一度の作業で適用できそう！
だけどこの操作をすると何が設定されているの？と思ったので調べてみた！

# 公式ドキュメントで推奨されているマネジメントコンソールの [Systems Manager] => [フリートマネージャー] からの設定について
マネジメントコンソールのフリートマネージャーから設定した場合、実際はSystems Managerのステートマネージャーという機能に設定がされており、マネジメントコンソールで確認できる。
![](/images/automating-updates-to-ssm-agent-with-cfn-stacksets/state-manager-console-after-automating-updates-to-ssm-agent.png)

ステートマネージャーの細かい説明は今回はしないが、関連付け(Assosiations)という自動で実行するSSMドキュメントと対象のサーバーを紐付けた一連の設定が作成される。
つまり今回作成された以下の関連付け(Assosiations)の設定内容をCloudFormationのテンプレートファイルで用意できればOKである👌
![](/images/automating-updates-to-ssm-agent-with-cfn-stacksets/state-manager-console-automating-updates-to-ssm-agent-assosiation-details.png)

# 作成したCloudFormationのテンプレートファイル
マネジメントコンソールのフリートマネージャーから設定したときに作成されたステートマネージャーの関連付け(Assosiations)の内容を確認し、それと照らし合わせて作成したテンプレートファイルは以下である。

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

一番重要なところは`AssociationName`を`SystemAssociationForSsmAgentUpdate`にしておくことである。フリートマネージャーのマネジメントコンソールで設定する場合は`"SystemAssociationForSsmAgentUpdate"`という名前で作成される。この名前で作成するとフリートマネージャーのマネジメントコンソール上でも設定済み状態として認識されるようである。

`MaxConcurrency`, `MaxErrors`, `ScheduleExpression`はフリートマネージャーのマネジメントコンソールで設定した場合の値にしているが、要件によって自由に変更しても良いと思う。
`WaitForSuccessTimeoutSeconds`はCloudFormationからの適用の場合に関係する値なのでこちらも変更可。

# CloudFormationのStackSetsで適用しよう！
あとは先ほど作成したテンプレートファイルがあればCloudFormationのStackSetsで複数リージョンや複数アカウントに一気に適用するだけ！
StackSetsを利用する場合は2パターンあり、事前にロールの設定やOrganizationsの信頼関係などが必要になるので要確認↓↓↓
https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/stacksets-prereqs.html


# どうでも良いけど気になったので試してみたシリーズ
## で、CloudFormationで適用した場合はフリートマネージャーのマネジメントコンソールはどうなるの？
[こちらのように](automating-updates-to-ssm-agent-with-cfn-stacksets#マネジメントコンソールのフリートマネージャーから「自動更新」適用後の状態)適用した後の状態になっている。

## フリートマネージャーのマネジメントコンソールでの設定とCloufFormationからの適用両方してしまったらどうなるの？
それぞれで`SystemAssociationForSsmAgentUpdate`という名前で関連付け(Assosiation)が作成される。関連付けIDが違うものができるため、同じような関連付け(Assosiation)ができるだけである。

## `AssociationName`を`SystemAssociationForSsmAgentUpdate`ではないもので作成したらどうなるの？
自動更新の設定はステートマネージャーの関連付け(Assosiation)で定義されて実行されるが、フリートマネージャーのマネジメントコンソールからは[こちらのように](automating-updates-to-ssm-agent-with-cfn-stacksets#マネジメントコンソールのフリートマネージャーから「自動更新」適用前の状態)適用できる状態のままになっている。

## マネジメントコンソールの [ステートマネージャー] から`AssociationName`を`SystemAssociationForSsmAgentUpdate`にしてAssosicationを作成したらどうなるの？
[こちらのように](automating-updates-to-ssm-agent-with-cfn-stacksets#マネジメントコンソールのフリートマネージャーから「自動更新」適用後の状態)適用した後の状態になっている。

## `AssociationName`を`SystemAssociationForSsmAgentUpdate`で紐付けるドキュメントを`AWS-UpdateSSMAgent`以外にするとどうなるの？
ドキュメントを`AWS-UpdateEC2Config`にしたが、[こちらのように](automating-updates-to-ssm-agent-with-cfn-stacksets#マネジメントコンソールのフリートマネージャーから「自動更新」適用後の状態)適用した後の状態になっている。ここまでの操作を含めての動きでは、`SystemAssociationForSsmAgentUpdate`という名前でステートマネージャーに関連付け(Assosiate)が作成されているかどうかだけでマネジメントコンソールのUIの表示が変わるようである👀

# おわりに
わざわざまとめなくてもやっている人たちはやっているかもしれないが、自分の中での整理やマネジメントコンソールの表示がどうなるかなどの調査もできた٩( ᐛ )و