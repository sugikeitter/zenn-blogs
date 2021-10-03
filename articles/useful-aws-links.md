---
title: "AWS 参考リンク集"
emoji: "🔗"
type: "idea" # tech: 技術記事 / idea: アイデア
topics: ["aws"]
published: false
---

AWS ユーザーガイドやデベロッパーガイド以外で役立つリンク集をまとめています。随時更新します。

# AWS について

## 全般
|URL||
|---|---|
|[AWS (アマゾン ウェブ サービス) とは？](https://aws.amazon.com/jp/what-is-aws/)| AWS の紹介。よりメリットについて言及してた[AWS の クラウドが選ばれる 10 の理由](https://aws.amazon.com/jp/aws-ten-reasons/)のサイトもある。|
|[AWS グローバルインフラストラクチャ](https://aws.amazon.com/jp/about-aws/global-infrastructure/)| AWS グローバルインフラストラクチャの最新情報やメリットなど。エッジロケーションの位置は [CloudFront の特徴ページ](https://aws.amazon.com/jp/cloudfront/features/)に記載されている。|
|[AWS Well-Architected のポータルサイト](https://aws.amazon.com/jp/architecture/well-architected/)| AWS Well-Architected フレームワーク、レンズ、Tool などの情報がまとめられている。|
|[What’s New at AWS (English)](https://aws.amazon.com/new/)| AWS の最新リリース情報が更新さ絵ている。[日本語版のはこちら](https://aws.amazon.com/jp/new/)。|
|[よくある質問](https://aws.amazon.com/jp/faqs/)| サービスごとによくある質問ページが用意されていて、利用する時に知りたい情報が多く書かれている |
|[AWS サポート - ナレッジセンター](https://aws.amazon.com/jp/premiumsupport/knowledge-center/)| AWS のお客様から最も頻繁に寄せられるご質問とご要望をいくつかご紹介しているサイト。|
|[AWSサービス別資料](https://aws.amazon.com/jp/aws-jp-introduction/aws-jp-webinar-service-cut/)| 各サービスごとに基礎から発展的な知識まで素早く知るのに役立つ資料集|

## 公式ブログ
|URL||
|---|---|
|[AWS Blog (English)](https://aws.amazon.com/blogs/?nc1=h_ls)| 英語のブログ。記事の量がかなり充実している。|
|[Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/)| AWS の日本ブログ。[AWS Blog (English)](https://aws.amazon.com/blogs/?nc1=h_ls) から一部ピックアップして翻訳されているものもある。|
|[AWS Startup ブログ](https://aws.amazon.com/jp/blogs/startup/)| 日本のスタートアップ関連の情報。|
|[AWS JAPAN APN ブログ](https://aws.amazon.com/jp/blogs/psa/)| 日本の APN(AWS Partner Network) 関連の情報。|
|[変化を求めるデベロッパーを応援するウェブマガジン - builders.flash](https://aws.amazon.com/jp/builders-flash/)| 身近なテーマで実践的なクラウドベストプラクティスを解説する記事や、幅広い開発インタビューをお届けする AWS のデベロッパー向けウェブマガジン。少しゆるめの記事が多い。|

## YouTube チャンネル
|URL||
|---|---|
|[Amazon Web Services Japan 公式](https://www.youtube.com/channel/UCnjKWUK2t5QJYfeqqilhJhQ)| 日本で行われた Summit のセッションごとの動画、AWS Black Belt Online Seminar シリーズ、活用事例、よくある質問に対して AWS サポートのエンジニアの回答など。|
|[AWS Startup Community](https://www.youtube.com/channel/UCPq5x-mI_knbOdmwEeuWtVg/featured)| AWS を利用しているスタートアップ同士の交流や経験の共有を目的とたコミュニティのチャンネル。|
|[Amazon Web Services (English)](https://www.youtube.com/channel/UCd6MoB9NC6uYN2grvUNT-Zg)| The official YouTube channel for Amazon Web Services (AWS).|
|[AWS Online Tech Talks (English)](https://www.youtube.com/channel/UCT-nPlVzJI-ccQXlxjSvJmw)| AWS の特定のサービスや技術について深堀した動画が多数。|
|[Serverless Land (English)](https://www.youtube.com/c/ServerlessLand)| サーバーレス関連の情報を扱ったチャンネル。|

## リファレンスアーキテクチャ
|URL||
|---|---|
|[AWS クイックスタート](https://aws.amazon.com/jp/quickstart/)| AWS クラウドでの自動化された、標準的なデプロイメントの設計図や CloudFormation テンプレートなど。|
|[AWS ソリューションライブラリ](https://aws.amazon.com/jp/solutions/)| AWS クラウド用の検証済みテクノロジーソリューションの設計図や CloudFormation テンプレートなど。クイックスタートの情報と重複しているものもある。|
|[The Amazon Builders' Library](https://aws.amazon.com/jp/builders-library/)| Amazon がテクノロジーを開発、設計、リリース、運用する方法を説明する記事のコレクション。|

## AWS 関連の GitHub リポジトリ
|URL||
|---|---|
|https://github.com/aws| AWS の CLI, SDK, CDK, SAM などの OSS ツールなど。|
|https://github.com/awslabs| ↑以外の AWS の OSS ツールなど。|
|https://github.com/aws-samples| AWS の利用例やワークショップなど。 |
|https://github.com/boto| AWS CLI のコアロジックや AWS SDK for Python のコード。|
|https://github.com/aws-amplify| AWS Amplify の独立したリポジトリ。|
|https://github.com/aws-containers| AWS コンテナ関連の独立したリポジトリ。ツールや利用例、ワークショップなど。|

## おまけ
|URL||
|---|---|
|[AWS Stash](https://awsstash.com/)|公式ではないがAWS関連資料が高速に検索できるサイト。|

# サービス

:::message
**Lv.** が設定されているものは、[こちら](https://pages.awscloud.com/rs/112-TZM-766/images/seminar_level_2020.pdf)の表を参考に判断している
> |Lv.||
> |---|---|
> |`100`| 入門 |
> |`200`| 中級 |
> |`300`| アドバンスト |
> |`400`| エキスパート |
:::

## App Runner
|Lv.|タイトル|動画URL||
|---|---|---|---|
|`200`|AWS App Runner とは？ - AWS Expert Online for JAWS-UG #16|[`YouTube`](https://www.youtube.com/watch?v=--o2HwfnFiY)| App Runner の使い方とメリットを、デモを通して紹介。|

## CloudFormation
|Lv.|タイトル|動画URL||
|---|---|---|---|
|`200`| [AWS Organizations × CloudFormation StackSetsの組み合わせが素晴らしい - プログラマでありたい](https://blog.takuros.net/entry/2020/03/25/093247)| -| StackSets の利用例とメリットなど。|

## CloudTrail
|Lv.|タイトル|動画URL||
|---|---|---|---|
|`200`| [AWS CloudTrail ログをモニタリングするためのベストプラクティス - Datadog](https://www.datadoghq.com/ja/blog/monitoring-cloudtrail-logs/)| -| AWS CloudTrail 監査ログの構造、監視する重要な CloudTrail ログ、Datadog との連携など。|

## Cognito
|Lv.|タイトル|動画URL||
|---|---|---|---|
|`100`| [アプリにユーザー認証機能を簡単に追加 !「Amazon Cognito」をグラレコで解説 - builders.flash](https://aws.amazon.com/jp/builders-flash/202103/awsgeek-cognito/)| -| Cognito の概要がわかりやすい絵と共に解説されている。|
|`200`| [AWS再入門ブログリレー Amazon Cognito編 - DevelopersIO](https://dev.classmethod.jp/articles/re-introduction-2020-amazon-cognito/)| -| ユーザープール、ID プールの利用パターンが解説されている。|
|`200`| [Cognitoのサインイン時に取得できる、IDトークン・アクセストークン・更新トークンを理解する - DevelopersIO](https://dev.classmethod.jp/articles/study-tokens-of-cognito-user-pools/)| -| Cognito で利用するトークンの解説。|

## Config
|Lv.|タイトル|動画URL||
|---|---|---|---|
|`200`| [やらないという選択肢はない　AWS Configを用いたマルチアカウント・マルチリージョンでのリソース把握とコンプライアンス維持 - ログミーTech](https://logmi.jp/tech/articles/323894)| -| AWS Configを用いたマルチアカウント・マルチリージョンでのリソース把握とコンプライアンス維持への取り組み|

## Control Tower
|Lv.|タイトル|動画URL||
|---|---|---|---|
|`200`| [AWS ソリューションプロバイダー向け AWS Control Tower のベストプラクティス - AWS JAPAN APN ブログ](https://aws.amazon.com/jp/blogs/psa/aws-control-tower-best-practices-for-aws-solution-providers/)| -| ソリューションプロバイダープログラムのお客様が AWS Control Tower を導入から継続的な運用までのプロセスを機能させる方法。|
|`200`| [AWS Control Towerの嬉しいポイントと注意ポイント - NRIネットコム Design and Tech Blog](https://tech.nri-net.com/entry/controltower-kms)| -| AWS Control Tower を実際に利用するときのポイント。|

## DynamoDB
|Lv.|タイトル|動画URL||
|---|---|---|---|
|`200`| Amazon DynamoDB Deep Dive - AWS Summit Tokyo 2019|[`YouTube`](https://www.youtube.com/watch?v=16RYHfe89WY)| DynamoDB の基本から内部構造の詳細、デザインパターンなどの発展的な情報まで。|
|`300`| [RDB と DynamoDB のデータベース設計プロセスの違い](https://www.slideshare.net/AmazonWebServicesJapan/db-20190905/18)| -| 2019/09/05 に開催された AWS のイベント、「イチから理解するサーバーレスアプリ開発」における講演資料の一つ。|

## EBS
|Lv.|タイトル|動画URL||
|---|---|---|---|
|`200`| [「Amazon EBS 完全に理解した」あなたに贈る Amazon EBS 再入門 - AWS Summit Online 2020](https://pages.awscloud.com/rs/112-TZM-766/images/AWS-20_AWS_Summit_Online_2020_STG02.pdf)| -| EBS の基本的な使い方や、ボリュームタイプの選択基準など。|
|`200`| [Amazon Elastic Block Store (EBS) によるイノベーションの加速 - AWS Summit Online 2021](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-40_AWS_Summit_Online_2021_STG01.pdf)|[`YouTube`](https://youtu.be/kbnlAb__Lgk)| 2021年時点での EBS ボリュームタイプやパフォーマンスなどの最新情報。|

## EC2
|Lv.|タイトル|動画URL||
|---|---|---|---|
|`100`| [空きキャパシティとスポット価格についてのわかりやすい図](https://www.slideshare.net/AmazonWebServicesJapan/20190306-aws-black-belt-online-seminar-amazon-ec2-149392937/18)| -|AWS Black Belt Online Seminar Amazon EC2 スポットインスタンス|
|`200`| [Amazon EC2 の進化の歴史から学ぶ EC2 入門 2019年版 - AWS Summit Tokyo 2019](https://pages.awscloud.com/rs/112-TZM-766/images/C2-06.pdf)|[`YouTube`](https://ww.youtube.com/watch?v=SbKLo5atgk4)| EC2 のインスタンスタイプや機能を時系列に紹介している。|
|`200`| [Amazon EC2インスタンスタイプの選び方ガイド - AWS Summit Tokyo 2019](https://pages.awscloud.com/rs/112-TZM-766/images/C2-07.pdf)|[`YouTube`](https://www.youtue.com/watch?v=Q1LUX8WMjHY)| [EC2 インスタンスのネーミングポリシー](https://pages.awscloud.com/rs/112-TZM-766/images/C2-07.pdf#page=14)と[追加機能のオプション表記](https://pages.awscloud.com/rs/112-TZM-766/images/C2-07.pdf#page=21)がわかりやすい。|
|`200`| [Amazon EC2 ことはじめ 〜あらゆるワークロードに対応する豊富な選択肢とコスト最適化オプション〜 - AWS Summit Online 2021](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-13_AWS_Summit_Online_2021_CMP01.pdf)|[`YouTube`](https://youtu.be/wD-KOWEmx5E)| [EC2インスタンスの選び方](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-13_AWS_Summit_Online_2021_CMP01.pdf#page=12)や、コストとキャパシティーの最適化など。[Savings Plans](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-13_AWS_Summit_Online_2021_CMP01.pdf#page=30)の解説図や[Savings Plans と RI の関係](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-13_AWS_Summit_Online_2021_CMP01.pdf#page=34)がわかりやすい。|

## Organizations
|Lv.|タイトル|動画URL||
|---|---|---|---|
|`200`| [AWS Organizationsを活用したマルチアカウントのセキュリティサービス使用方法 ～まとめ～ - fu3ak1's tech days](https://fu3ak1.hatenablog.com/entry/2021/01/28/002536)| -| Organizationsを活用したセキュリティサービスについての紹介。|
|`200`| [「進化し続けるインフラ」でありたい　リクルートのAWS基盤チームによるマルチアカウント管理 - ログミーTech](https://logmi.jp/tech/articles/323814)| -| 約90の AWS アカウントに対して横断的な管理、コスト配賦、共通機能の提供などの運用について。|

## IAM
|Lv.|タイトル|動画URL||
|---|---|---|---|
|`100`| [[AWS利用者必読] アクセスキー漏洩による不正利用について - DevelopersIO](https://dev.classmethod.jp/articles/unauthorized-use-of-aws-access-keys-due-to-leakage/)| -| アクセスキー利用の注意点について。|
|`200`| [【実録】アクセスキー流出、攻撃者のとった行動とその対策 - DevelopersIO](https://dev.classmethod.jp/articles/accesskey-leak/)| -| アクセスキーを利用してどのように不正な操作がされたかの経験談とその対策。|
|`200`| [AWS IAMの最小権限追求の旅 - プログラマでありたい](https://blog.takuros.net/entry/2020/07/06/081552)| -| IAMでのセキュリティのベストプラクティスを実際に行うための難しさや、SCPとPermission Boundary を利用する話。|

## Lambda
|Lv.|タイトル|動画URL||
|---|---|---|---|
|`200`| [API Gateway＋Lambdaでのステージ管理やCloudWatch Logsのログ運用のはなし - サーバーワークスエンジニアブログ](https://blog.serverworks.co.jp/tech/2017/02/01/apigateway-lambda-cloudwatchlogs/)| -| [API Gateway と Lambda のバージョン、エイリアスの関係の画像](https://cdn-ak.f.st-hatena.com/images/fotolife/s/serverworks/20200711/20200711162254.png)がわかりやすい。|
|`200`| [LambdaのDLQ(デッドレターキュー)とDestinations(非同期呼び出しの宛先指定)を比較してみた - DevelopersIO](https://dev.classmethod.jp/articles/lambda-dlq-vs-destinations/)| -| 非同期呼び出しのLambdaが処理失敗した場合の挙動の設定。|
|`300`| [AWS Summit Online JAPAN 2020 - Let’s dive deep into AWS Lambda error handling](https://pages.awscloud.com/rs/112-TZM-766/images/AWS-35_AWS_Summit_Online_2020_MAD01.pdf)| -| Lambda のエラー発⽣時のリトライ制御、エラー伝搬の回避、データ整合性の確保の方法。|

## RDS
|Lv.|タイトル|動画URL||
|---|---|---|---|
|`200`| [Amazon RDS アーキテクチャ概要](https://pages.awscloud.com/rs/112-TZM-766/images/01_RDS_Architecture.pdf)| -| [2020/10/15に開催された第2回 Amazon RDS Online Seminar](https://aws.amazon.com/jp/blogs/news/amazon-rds-online-seminar2-qa-202011/)の資料。|
|`200`| [Amazon Aurora アーキテクチャ概要](https://pages.awscloud.com/rs/112-TZM-766/images/01_Amazon%20Aurora%20%E3%82%A2%E3%83%BC%E3%82%AD%E3%83%86%E3%82%AF%E3%83%81%E3%83%A3%E6%A6%82%E8%A6%81.pdf)| -| [2020/09/10に開催された第1回 Amazon RDS Online Seminar](https://aws.amazon.com/jp/blogs/news/amazon-rds-online-seminar1-qa-202009/)の資料。[Aurora が⾼いパフォーマンスを発揮する理由](https://pages.awscloud.com/rs/112-TZM-766/images/01_Amazon%20Aurora%20%E3%82%A2%E3%83%BC%E3%82%AD%E3%83%86%E3%82%AF%E3%83%81%E3%83%A3%E6%A6%82%E8%A6%81.pdf#page=31)も。|
|`200`| [Amazon RDS Online Seminar 「忘れちゃいけない！Amazon RDS/Amazon Aurora のアップグレードとその方法」資料・動画及び QA 公開 - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/amazon-rds-online-seminar-20210617/)| -| 2021/6/17に開催した Amazon RDS Online Seminar「忘れちゃいけない！Amazon RDS/Amazon Aurora のアップグレードとその方法」の資料・動画。|
|`300`| [Aurora MySQL のバックアップは本当にそれでいいのだろうか？ - CyberAgent Developers Blog](https://developers.cyberagent.co.jp/blog/archives/29925/)| -| バイナリログである特定のクエリまで戻す方法と、バックトラック / ポイントインタイムリカバリで日時指定で復元する方法。|
|`300`| [Amazon RDS for Oracle で実現するエンタープライズ領域における高性能/高可用性構成 - AWS Summit Online 2021](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-49_AWS_Summit_Online_2021_RDSforOracle_Enterprise.pdf)|[`YouTube`](https://www.youtube.com/watch?v=qXspvi86GHg)| Oracle RAC を利用できない RDS で可用性高める方法。|
|`300`| [Amazon Aurora はこう使え！貴方にだけ便利な使い方教えます！ - AWS Summit Tokyo 2020](https://pages.awscloud.com/rs/112-TZM-766/images/AWS-25_AWS_Summit_Online_2020_DAT01.pdf)| -| Database cloning による環境の複製や復旧、監視、分析のための機能など。|

## Route53
|Lv.|タイトル|動画URL||
|---|---|---|---|
|`200`|DNS Design Using Amazon Route 53 - AWS Online Tech Talks (English)|[`YouTube`](https://www.youtube.com/watch?v=2y_RBjDkRgY)||
|`200`| [[レポート] ARC408: Route 53 SLA 100% の舞台裏 (Under the Hood of Amazon Route 53) #reinvent - DevelopersIO](https://dev.classmethod.jp/articles/report-reinvent-2018-1128-arc408/)| -| Route 53 を如何に大規模かつ SLA 100% のサービスとして AWS エンジニアリングチームが運営しているかの説明。|
|`300`| [シャッフルシャーディングを使ったワークロードの分離](https://aws.amazon.com/jp/builders-library/workload-isolation-using-shuffle-sharding/)| -| DDoS 攻撃への対処としてのシャッフルシャーディングの解説。|

## Systems Manager
|Lv.|タイトル|動画URL||
|---|---|---|---|
|`200`| [AWS Systems Manager(SSM) の数多い機能群を攻略するための図を書いてみた 2021 - DevelopersIO](https://dev.classmethod.jp/articles/all-ssm-capabilities-2021/)| -| Systems Manager の機能一覧が把握しやすい図。|
|`200`| [AWSでSSMエージェントの自動更新をCloudFormationのスタックセット(StackSets)で複数のリージョンやアカウントに適用](https://zenn.dev/sugikeitter/articles/automating-updates-to-ssm-agent-with-cfn-stacksets)| -| マルチアカウント環境などで全てのサーバーのSSMエージェントの自動更新させる方法。|
|`300`| [AWS IAMの安全な管理方法 · DeNA Engineers' Blog](https://engineer.dena.com/posts/2019.12/aws-iam-management/)| -| IAM ロールが利用できないシステムからAWSサービスへのアクセス時に、定期的にIAMユーザのシークレットアクセスキーのローテートを行う方法。|

## S3
|Lv.|タイトル|動画URL||
|---|---|---|---|
|`400`| [Diving Deep on S3 Consistency (English)](https://www.allthingsdistributed.com/2021/04/s3-strong-consistency.html)| -| S3で整合性を保つための仕組みを解説。|

## SQS
|Lv.|タイトル|動画URL||
|---|---|---|---|
|`200`| SQS 標準キューのCLIを利用した動作デモ|[`YouTube`](https://www.youtube.com/watch?v=8cAk1_GSV0g&t=336s)| 動画なのでプロデューサー・キュー・コンシューマーの関係がわかりやすい。順序保証がないことや、コンシューマーを増やすことで処理量が線形的に増えていくことがわかる。|
|`200`| SQS FIFOキューのCLIを利用した動作デモ|[`YouTube`](https://www.youtube.com/watch?v=8cAk1_GSV0g&t=660s)| 標準キューと比較してコンシューマーが増えても処理量が線形的に増えるわけではないことや、並列化をしたい場合のグループID利用、プロデューサーからの重複排除が可能なことがわかる。|

## SSO
|Lv.|タイトル|動画URL||
|---|---|---|---|
|`200`| [Azure AD と AWS SSOの連携 - fu3ak1's tech days](https://fu3ak1.hatenablog.com/entry/2020/12/20/000622)| -| IdP として Azure Active Directory を利用したAWS SSO の構築方法。|

## StepFunctions
|Lv.|タイトル|動画URL||
|---|---|---|---|
|`300`| [分散システムにおけるSagaパターンのAWS Step Functions による実装 #AWSDevDay - Speaker Deck](https://speakerdeck.com/fatsushi/fen-san-sisutemuniokerusagapatanfalseaws-step-functions-niyorushi-zhuang-number-awsdevday)| -| Saga パターンについての話と、Step Functions によるエラーハンドリングとリトライ、[e-コマースの注文処理のサンプル実装例](https://github.com/aws-samples/aws-step-functions-long-lived-transactions)など。|


# カテゴリ別

## サーバーレス / Serverless
|Lv.|タイトル|動画URL||
|---|---|---|---|
||https://serverlessland.com/||
