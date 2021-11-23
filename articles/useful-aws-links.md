---
title: "AWS お役立ちリンク集"
emoji: "🔗"
type: "idea" # tech: 技術記事 / idea: アイデア
topics: ["aws"]
published: true
---

:::message alert
最新の情報は [AWS の公式ドキュメント](https://docs.aws.amazon.com/)をご確認ください。
:::

AWS ユーザーガイドやデベロッパーガイド以外で役立つリンク集をまとめています。（随時更新）

:::message
**Lv.** は[こちらの表](https://pages.awscloud.com/rs/112-TZM-766/images/seminar_level_2020.pdf)を参考に独自で以下のように設定しています。
:::
> |Lv.||
> |---|---|
> |`100`| 入門 |
> |`200`| 中級 |
> |`300`| アドバンスト |
> |`400`| エキスパート |
> |`---`| 事例など |

# AWS について

## 全般
|URL|備考|
|---|---|
|[AWS (アマゾン ウェブ サービス) とは？](https://aws.amazon.com/jp/what-is-aws/)| AWS の紹介。よりメリットについて言及してた[AWS の クラウドが選ばれる 10 の理由](https://aws.amazon.com/jp/aws-ten-reasons/)のサイトもある。|
|[AWS グローバルインフラストラクチャ](https://aws.amazon.com/jp/about-aws/global-infrastructure/)| AWS グローバルインフラストラクチャの最新情報やメリットなど。[AWS のデータセンターのページ](https://aws.amazon.com/jp/compliance/data-center/data-centers/)や、エッジロケーションの位置が記載された [CloudFront の特徴](https://aws.amazon.com/jp/cloudfront/features/)のページも用意されている。|
|[AWS Well-Architected のポータルサイト](https://aws.amazon.com/jp/architecture/well-architected/)| AWS Well-Architected フレームワーク、レンズ、Tool などの情報がまとめられている。|
|[What’s New at AWS (English)](https://aws.amazon.com/new/)| AWS の最新リリース情報が更新れている。[日本語版はこちら](https://aws.amazon.com/jp/new/)。|
|[よくある質問](https://aws.amazon.com/jp/faqs/)| サービスごとによくある質問ページが用意されていて、利用する時に知りたい情報が多く書かれている |
|[AWS サポート - ナレッジセンター](https://aws.amazon.com/jp/premiumsupport/knowledge-center/)| AWS のお客様から最も頻繁に寄せられるご質問とご要望をいくつかご紹介しているサイト。|
|[AWSサービス別資料](https://aws.amazon.com/jp/aws-jp-introduction/aws-jp-webinar-service-cut/)| 各サービスごとに基礎から発展的な知識まで素早く知るのに役立つ資料集|

## 公式ブログ
|URL|備考|
|---|---|
|[AWS Blog (English)](https://aws.amazon.com/blogs/?nc1=h_ls)| 英語のブログ。記事の量がかなり充実している。|
|[Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/)| AWS の日本ブログ。[AWS Blog (English)](https://aws.amazon.com/blogs/?nc1=h_ls) から一部ピックアップして翻訳されているものもある。|
|[AWS Startup ブログ](https://aws.amazon.com/jp/blogs/startup/)| 日本のスタートアップ関連の情報。|
|[AWS JAPAN APN ブログ](https://aws.amazon.com/jp/blogs/psa/)| 日本の APN(AWS Partner Network) 関連の情報。|
|[変化を求めるデベロッパーを応援するウェブマガジン - builders.flash](https://aws.amazon.com/jp/builders-flash/)| 身近なテーマで実践的なクラウドベストプラクティスを解説する記事や、幅広い開発インタビューをお届けする AWS のデベロッパー向けウェブマガジン。少しゆるめの記事が多い。|

## YouTube チャンネル
|URL|備考|
|---|---|
|[Amazon Web Services Japan 公式](https://www.youtube.com/channel/UCnjKWUK2t5QJYfeqqilhJhQ)| 日本で行われた Summit のセッションごとの動画、AWS Black Belt Online Seminar シリーズ、活用事例、よくある質問に対して AWS サポートのエンジニアの回答など。|
|[AWS Startup Community](https://www.youtube.com/channel/UCPq5x-mI_knbOdmwEeuWtVg/featured)| AWS を利用しているスタートアップ同士の交流や経験の共有を目的とたコミュニティのチャンネル。|
|[Amazon Web Services (English)](https://www.youtube.com/channel/UCd6MoB9NC6uYN2grvUNT-Zg)| The official YouTube channel for Amazon Web Services (AWS).|
|[AWS Online Tech Talks (English)](https://www.youtube.com/channel/UCT-nPlVzJI-ccQXlxjSvJmw)| AWS の特定のサービスや技術について深堀した動画が多数。|
|[Serverless Land (English)](https://www.youtube.com/c/ServerlessLand)| サーバーレス関連の情報を扱ったチャンネル。|

## リファレンスアーキテクチャ
|URL|備考|
|---|---|
|[AWS クイックスタート](https://aws.amazon.com/jp/quickstart/)| AWS クラウドでの自動化された、標準的なデプロイメントの設計図や CloudFormation テンプレートなど。|
|[AWS ソリューションライブラリ](https://aws.amazon.com/jp/solutions/)| AWS クラウド用の検証済みテクノロジーソリューションの設計図や CloudFormation テンプレートなど。クイックスタートの情報と重複しているものもある。|
|[The Amazon Builders' Library](https://aws.amazon.com/jp/builders-library/)| Amazon がテクノロジーを開発、設計、リリース、運用する方法を説明する記事のコレクション。|

## AWS 関連の GitHub リポジトリ
|URL|備考|
|---|---|
|https://github.com/aws| AWS の CLI, SDK, CDK, SAM などの OSS ツールなど。|
|https://github.com/awslabs| ↑以外の AWS の OSS ツールなど。|
|https://github.com/awsdocs| ユーザーガイドなどのドキュメントや [SDK のサンプルコード](https://github.com/awsdocs/aws-doc-sdk-examples)など。|
|https://github.com/aws-samples| AWS の利用例やワークショップなど。 |
|https://github.com/boto| AWS CLI のコアロジックや AWS SDK for Python のコード。|
|https://github.com/aws-amplify| AWS Amplify の独立したリポジトリ。|
|https://github.com/aws-containers| AWS コンテナ関連の独立したリポジトリ。ツールや利用例、ワークショップなど。|

## AWS SDK ドキュメント
|URL|備考|
|---|---|
| [AWS SDK for .NET V3 API](https://docs.aws.amazon.com/sdkfornet/v3/apidocs/index.html)| シンプルな API ドキュメント。|
| [AWS SDK for Java](https://sdk.amazonaws.com/java/api/latest/)| javadoc を HTML にした Java ユーザーにはお馴染みの形式。|
| [AWS SDK for Python (Boto3)](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html)| 1ページの情報量が多いので、少し表示が重いこともあるので注意。|

## おまけ
|URL|備考|
|---|---|
|[AWS Stash](https://awsstash.com/)|公式ではないがAWS関連資料が高速に検索できるサイト。|
| `site:d1.awsstatic.com`<br>`site:pages.awscloud.com`| Google 検索のキーワードに追加すると、AWS イベントの発表資料の PDF が多く検索結果にヒットするので便利。`site:d0.awsstatic.com`もあるけど少し古め？かも。両方のドメインをまとめて検索したい場合は`<検索ワード> site:pages.awscloud.com OR site:d1.awsstatic.com`で検索可能。|

# サービス別

## API Gateway
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`300`| [Amazon API Gateway は何をしてるのか - DevelopersIO](https://dev.classmethod.jp/articles/what-does-amazon-api-gateway-do/)| -| API Gateway の機能が網羅的に纏まっている。|


## App Runner
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| AWS App Runner とは？ - AWS Expert Online for JAWS-UG #16| [`YouTube`](https://www.youtube.com/watch?v=--o2HwfnFiY)| App Runner の使い方とメリットを、デモを通して紹介。|

## Client VPN
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [AWS Client VPN のリソースとパラメータを一枚絵にまとめつつ過去のエントリもまとめてみた - DevelopersIO](https://dev.classmethod.jp/articles/aws-client-vpn-perfect-understand-2/)| -| 証明書や認証周りなども含めて整理されている。|
|`---`| [AWS 導入事例：コクヨ株式会社 - AWS](https://aws.amazon.com/jp/solutions/case-studies/kokuyo-serverworks/)| -| Direct Connect は利用している状態から、1,000 名規模のリモートワーク環境を10日間で構築した話。|


## CloudFormation
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [AWS Organizations × CloudFormation StackSetsの組み合わせが素晴らしい - プログラマでありたい](https://blog.takuros.net/entry/2020/03/25/093247)| -| StackSets の利用例とメリットなど。|

## CloudFront
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`300`| [Visitor PrioritizationソリューションをCloudFront Functionsを使って実装するための考慮点 - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/visitor-prioritization-by-cloudfront-functions/)| -| CloudFront Functions　を利用したユーザーの優先制御、流量制御を行うための静的なウェイティングルームページにに誘導するソリューション。|

## CloudHSM
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [ハードウェアセキュリティモジュール - ITソリューションのTIS株式会社](https://www.tis.jp/service_solution/safenet_HSM/)
|`---`| [AWSセキュリティ事例 -  ITソリューションのTIS株式会社](https://www.tis.jp/special/aws_security/)| -| 株式会社日本カードネットワークが決済ネットワークの J-Helix システムで、取り扱うデータの暗号化と暗号鍵の管理に CloudHSM と KMS を利用した事例。|

## CloudTrail
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [AWS CloudTrail ログをモニタリングするためのベストプラクティス - Datadog](https://www.datadoghq.com/ja/blog/monitoring-cloudtrail-logs/)| -| AWS CloudTrail 監査ログの構造、監視する重要な CloudTrail ログ、Datadog との連携など。|

## Cognito
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [アプリにユーザー認証機能を簡単に追加 !「Amazon Cognito」をグラレコで解説 - builders.flash](https://aws.amazon.com/jp/builders-flash/202103/awsgeek-cognito/)| -| Cognito の概要がわかりやすい絵と共に解説されている。|
|`200`| [AWS再入門ブログリレー Amazon Cognito編 - DevelopersIO](https://dev.classmethod.jp/articles/re-introduction-2020-amazon-cognito/)| -| ユーザープール、ID プールの利用パターンが解説されている。|
|`200`| [Cognitoのサインイン時に取得できる、IDトークン・アクセストークン・更新トークンを理解する - DevelopersIO](https://dev.classmethod.jp/articles/study-tokens-of-cognito-user-pools/)| -| Cognito で利用するトークンの解説。|

## Control Tower
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [AWS ソリューションプロバイダー向け AWS Control Tower のベストプラクティス - AWS JAPAN APN ブログ](https://aws.amazon.com/jp/blogs/psa/aws-control-tower-best-practices-for-aws-solution-providers/)| -| ソリューションプロバイダープログラムのお客様が AWS Control Tower を導入から継続的な運用までのプロセスを機能させる方法。|
|`200`| [AWS Control Towerの嬉しいポイントと注意ポイント - NRIネットコム Design and Tech Blog](https://tech.nri-net.com/entry/controltower-kms)| -| AWS Control Tower を実際に利用するときのポイント。|
|`300`| [Architecture Overview - Customizations for AWS Control Tower](https://docs.aws.amazon.com/solutions/latest/customizations-for-aws-control-tower/architecture.html)| -| Control Tower のカスタマイズ方法の実装の一例についての紹介。[日本語の実装ガイド](https://aws.amazon.com/jp/solutions/implementations/customizations-for-aws-control-tower/)や[日本語のソリューション実装](https://controltower.aws-management.tools/ja/automation/cfct/)もある。|
|`300`| [「AWS Control Tower をカスタマイズして使ってみよう」というテーマでお話ししました #devio2021 - DevelopersIO](https://dev.classmethod.jp/articles/devio2021-cfcf/)|[`YouTube`](https://www.youtube.com/watch?v=j-7hN8te0Yo)| DynamoDB の基本から内部構造の詳細、デザインパターンなどの発展的な情報まで。| Control Tower でセットアップされないけれど初期設定に組み込みたいサービスのカスタマイズ方法の一例。|

## Direct Connect (DX)
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`---`| [AWS導入事例 株式会社ゼンリンデータコム様 - TOKAIコミュニケーションズ AWSソリューション](https://www.cloudsolution.tokai-com.co.jp/case/zenrin-datacom.html)| -| お客様データセンター <-> DXロケーション <-> AWS のネットワークへの接続の具体的な図がわかりやすい。|

## DynamoDB
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| Amazon DynamoDB Deep Dive - AWS Summit Tokyo 2019|[`YouTube`](https://www.youtube.com/watch?v=16RYHfe89WY)| DynamoDB の基本から内部構造の詳細、デザインパターンなどの発展的な情報まで。|
|`200`| [OPENREC.tv における Amazon DynamoDB を用いた スケーラブルなアプリケーション設計 - CyberZ, Inc.](https://pages.awscloud.com/rs/112-TZM-766/images/Session%204%20-%2020200825_CyberZ_OPENRECTV_Purpose-Built-Databases-Week-v2.pdf)| -| [プロビジョンド / オンデマンドのユースケース](https://pages.awscloud.com/rs/112-TZM-766/images/Session%204%20-%2020200825_CyberZ_OPENRECTV_Purpose-Built-Databases-Week-v2.pdf#page=27)がわかりやすい。|
|`300`| [RDB と DynamoDB のデータベース設計プロセスの違い](https://www.slideshare.net/AmazonWebServicesJapan/db-20190905/18)| -| 2019/09/05 に開催された AWS のイベント、「イチから理解するサーバーレスアプリ開発」における講演資料の一つ。|
|`300`| [Amazon DynamoDB deep dive: Advanced design patterns](https://pages.awscloud.com/rs/112-TZM-766/images/Session%203%20-%20purpose_built_database_DynamoDB_advancedDP_narita_rev.pdf) | -| NoSQL の正規化と非正規化によるデータモデリング / 複合key、階層的構造のデータ、リレーショナルなデータの表現などのデザインパターン / 実際のアプリケーションにおけるモデリング など。|
|`300`| [Amazon DynamoDB Under the Hood: How We Built a Hyper-Scale Database - AWS re:Invent 2018 (English)](https://www.slideshare.net/AmazonWebServices/amazon-dynamodb-under-the-hood-how-we-built-a-hyperscale-database-dat321-aws-reinvent-2018)| -| [データがパーティションごとに複数 AZ に分散されている図](https://www.slideshare.net/AmazonWebServices/amazon-dynamodb-under-the-hood-how-we-built-a-hyperscale-database-dat321-aws-reinvent-2018/17)がわかりやすい。|
|`---`| [PayPayでのDynamoDB活用事例について - Speaker Deck](https://speakerdeck.com/paypay/paypaydefalsedynamodbhuo-yong-shi-li-nituite)| -| PayPay の通知機能を実装するDB選定で DynamoDB を選択した理由など。|
|`---`| [サーバレスアーキテクチャで実現した M-1 グランプリ敗者復活戦投票システム](https://d0.awsstatic.com/events/jp/2017/summit/slide/D3T5-3.pdf)| -| M-1 グランプリ2016の敗者復活戦投票システムの DB に DynamoDB を選択した理由など。|

## EBS
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [「Amazon EBS 完全に理解した」あなたに贈る Amazon EBS 再入門 - AWS Summit Online 2020](https://pages.awscloud.com/rs/112-TZM-766/images/AWS-20_AWS_Summit_Online_2020_STG02.pdf)| -| EBS の基本的な使い方や、ボリュームタイプの選択基準など。|
|`200`| [Amazon Elastic Block Store (EBS) によるイノベーションの加速 - AWS Summit Online 2021](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-40_AWS_Summit_Online_2021_STG01.pdf)|[`YouTube`](https://youtu.be/kbnlAb__Lgk)| 2021年時点での EBS ボリュームタイプやパフォーマンスなどの最新情報。|

## EC2
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [空きキャパシティとスポット価格についてのわかりやすい図](https://www.slideshare.net/AmazonWebServicesJapan/20190306-aws-black-belt-online-seminar-amazon-ec2-149392937/18)| -|AWS Black Belt Online Seminar Amazon EC2 スポットインスタンス|
|`200`| [Amazon EC2 の進化の歴史から学ぶ EC2 入門 2019年版 - AWS Summit Tokyo 2019](https://pages.awscloud.com/rs/112-TZM-766/images/C2-06.pdf)|[`YouTube`](https://ww.youtube.com/watch?v=SbKLo5atgk4)| EC2 のインスタンスタイプや機能を時系列に紹介している。|
|`200`| [Amazon EC2インスタンスタイプの選び方ガイド - AWS Summit Tokyo 2019](https://pages.awscloud.com/rs/112-TZM-766/images/C2-07.pdf)|[`YouTube`](https://www.youtue.com/watch?v=Q1LUX8WMjHY)| [EC2 インスタンスのネーミングポリシー](https://pages.awscloud.com/rs/112-TZM-766/images/C2-07.pdf#page=14)と[追加機能のオプション表記](https://pages.awscloud.com/rs/112-TZM-766/images/C2-07.pdf#page=20)がわかりやすい。|
|`200`| [Amazon EC2 ことはじめ 〜あらゆるワークロードに対応する豊富な選択肢とコスト最適化オプション〜 - AWS Summit Online 2021](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-13_AWS_Summit_Online_2021_CMP01.pdf)|[`YouTube`](https://youtu.be/wD-KOWEmx5E)| [EC2インスタンスの選び方](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-13_AWS_Summit_Online_2021_CMP01.pdf#page=12)や、コストとキャパシティーの最適化など。[Savings Plans](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-13_AWS_Summit_Online_2021_CMP01.pdf#page=30)の解説図や[Savings Plans と RI の関係](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-13_AWS_Summit_Online_2021_CMP01.pdf#page=34)がわかりやすい。|

## EKS
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`300`| [EKS Anywhereのファーストインプレッション - inductor's blog](https://blog.inductor.me/entry/2021/09/10/031541)| -| |

## ELB
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`300`| [Network Load BalancerのターゲットグループにApplication Load Balancerを設定する - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/application-load-balancer-aws-privatelink-static-ip-addresses-network-load-balancer/)| -| ALB に固定 IP を設定したい場合の NLB + ALB 構成とユースケースについて。|

## Organizations
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [Organizing Your AWS Environment Using Multiple Accounts - Organizing Your AWS Environment Using Multiple Accounts](https://docs.aws.amazon.com/whitepapers/latest/organizing-your-aws-environment/organizing-your-aws-environment.html)| -| Organizations の OU の分け方などの推奨方法などがまとめられているホワイトペーパー。|
|`200`| [[AWS Organizations] SCP(サービスコントロールポリシー)の継承の仕組みを学ぼう - DevelopersIO](https://dev.classmethod.jp/articles/organizations-scp-inheritance/)| -| SCP の継承の考え方や、暗黙の Deny の概念が図でわかりやすい。|

## IAM
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [[AWS利用者必読] アクセスキー漏洩による不正利用について - DevelopersIO](https://dev.classmethod.jp/articles/unauthorized-use-of-aws-access-keys-due-to-leakage/)| -| アクセスキー利用の注意点について。|
|`200`| [【実録】アクセスキー流出、攻撃者のとった行動とその対策 - DevelopersIO](https://dev.classmethod.jp/articles/accesskey-leak/)| -| アクセスキーを利用してどのように不正な操作がされたかの経験談とその対策。|
|`200`| [AWS IAMの最小権限追求の旅 - プログラマでありたい](https://blog.takuros.net/entry/2020/07/06/081552)| -| IAMでのセキュリティのベストプラクティスを実際に行うための難しさや、SCPとPermission Boundary を利用する話。|

## Lambda
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [API Gateway＋Lambdaでのステージ管理やCloudWatch Logsのログ運用のはなし - サーバーワークスエンジニアブログ](https://blog.serverworks.co.jp/tech/2017/02/01/apigateway-lambda-cloudwatchlogs/)| -| [API Gateway と Lambda のバージョン、エイリアスの関係の画像](https://cdn-ak.f.st-hatena.com/images/fotolife/s/serverworks/20200711/20200711162254.png)がわかりやすい。|
|`200`| [LambdaのDLQ(デッドレターキュー)とDestinations(非同期呼び出しの宛先指定)を比較してみた - DevelopersIO](https://dev.classmethod.jp/articles/lambda-dlq-vs-destinations/)| -| 非同期呼び出しのLambdaが処理失敗した場合の挙動の設定。|
|`300`| [AWS Summit Online JAPAN 2020 - Let’s dive deep into AWS Lambda error handling](https://pages.awscloud.com/rs/112-TZM-766/images/AWS-35_AWS_Summit_Online_2020_MAD01.pdf)| -| Lambda のエラー発⽣時のリトライ制御、エラー伝搬の回避、データ整合性の確保の方法。|
|`300`| Operating Lambda: パフォーマンスの最適化 - Amazon Web Services ブログ| -| [<Part 1>](https://aws.amazon.com/jp/blogs/news/operating-lambda-performance-optimization-part-1/) 実行環境のライフサイクルと、コールドスタートの定義、測定、改善方法。[<Part 2>](https://aws.amazon.com/jp/blogs/news/operating-lambda-performance-optimization-part-2/) メモリ構成が Lambda のパフォーマンスに及ぼす影響と、静的初期化コードを最適化する方法。[<Part 3>](https://aws.amazon.com/jp/blogs/news/operating-lambda-performance-optimization-part-3/) Lambda 関数のパフォーマンス向上に役立つ関数のアーキテクチャとベストプラクティス。|
|`300`| [AWS Lambda Provisioned Concurrency Dive Deep & Practice - Speaker Deck](https://speakerdeck.com/_kensh/aws-lambda-provisioned-concurrency-dive-deep-and-practice)| -| Provisioned Concurrency のユースケースや活用方法など。|
|`300`| [大量リクエストを低コストでさばく AWS Lambda 関数を JVM で実現 - builders.flash☆](https://aws.amazon.com/jp/builders-flash/202110/jvm-lambda-function/?awsf.filter-name=*all)| -| Node.js, Python, Java での条件ごとのパフォーマンス比較や、GraalVM での native-image を利用する方法。|
|`400`| [知らなくても困らないけど、知ると楽しいAWS Lambdaの裏側の世界 #devio2021 - DevelopersIO](https://dev.classmethod.jp/articles/devio2021-awslambda-under-the-food/)| -| 実行環境である Firecracker や Lambda 関数の同期/非同期実行時のソフトウェアコンポーネント、コンテナイメージサポートの話など。|

## RDS
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [Amazon RDS アーキテクチャ概要](https://pages.awscloud.com/rs/112-TZM-766/images/01_RDS_Architecture.pdf)| -| [2020/10/15に開催された第2回 Amazon RDS Online Seminar](https://aws.amazon.com/jp/blogs/news/amazon-rds-online-seminar2-qa-202011/)の資料。|
|`200`| [Amazon Aurora アーキテクチャ概要](https://pages.awscloud.com/rs/112-TZM-766/images/01_Amazon%20Aurora%20%E3%82%A2%E3%83%BC%E3%82%AD%E3%83%86%E3%82%AF%E3%83%81%E3%83%A3%E6%A6%82%E8%A6%81.pdf)| -| [2020/09/10に開催された第1回 Amazon RDS Online Seminar](https://aws.amazon.com/jp/blogs/news/amazon-rds-online-seminar1-qa-202009/)の資料。[Aurora が⾼いパフォーマンスを発揮する理由](https://pages.awscloud.com/rs/112-TZM-766/images/01_Amazon%20Aurora%20%E3%82%A2%E3%83%BC%E3%82%AD%E3%83%86%E3%82%AF%E3%83%81%E3%83%A3%E6%A6%82%E8%A6%81.pdf#page=31)も。|
|`200`| [Amazon RDS Online Seminar 「忘れちゃいけない！Amazon RDS/Amazon Aurora のアップグレードとその方法」資料・動画及び QA 公開 - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/amazon-rds-online-seminar-20210617/)| -| 2021/6/17に開催した Amazon RDS Online Seminar「忘れちゃいけない！Amazon RDS/Amazon Aurora のアップグレードとその方法」の資料・動画。|
|`300`| [Aurora MySQL のバックアップは本当にそれでいいのだろうか？ - CyberAgent Developers Blog](https://developers.cyberagent.co.jp/blog/archives/29925/)| -| バイナリログである特定のクエリまで戻す方法と、バックトラック / ポイントインタイムリカバリで日時指定で復元する方法。|
|`300`| [Amazon RDS for Oracle で実現するエンタープライズ領域における高性能/高可用性構成 - AWS Summit Online 2021](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-49_AWS_Summit_Online_2021_RDSforOracle_Enterprise.pdf)|[`YouTube`](https://www.youtube.com/watch?v=qXspvi86GHg)| Oracle RAC を利用できない RDS で可用性高める方法。|
|`300`| [Amazon Aurora はこう使え！貴方にだけ便利な使い方教えます！ - AWS Summit Tokyo 2020](https://pages.awscloud.com/rs/112-TZM-766/images/AWS-25_AWS_Summit_Online_2020_DAT01.pdf)| -| Database cloning による環境の複製や復旧、監視、分析のための機能など。|
|`---`| [AWS 導入事例：任天堂株式会社、株式会社ディー・エヌ・エー](https://aws.amazon.com/jp/solutions/case-studies/nintendo-dena-2020/)| -| 『マリオカート ツアー』の DB に Amazon Aurora を採用。本番リリース当日に使用した Amazon Aurora のクラスタ数は 600 で、インスタンスは 1,200 台。以降、世界中からトラフィックが集中し、Amazon Aurora 全体の 1 秒あたりのクエリ数は最大で約 30 万を記録、データ量も 1 ヶ月で 30TB まで達した。|

## Route53
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`|DNS Design Using Amazon Route 53 - AWS Online Tech Talks (English)|[`YouTube`](https://www.youtube.com/watch?v=2y_RBjDkRgY)||
|`200`| [[レポート] ARC408: Route 53 SLA 100% の舞台裏 (Under the Hood of Amazon Route 53) #reinvent - DevelopersIO](https://dev.classmethod.jp/articles/report-reinvent-2018-1128-arc408/)| -| Route 53 を如何に大規模かつ SLA 100% のサービスとして AWS エンジニアリングチームが運営しているかの説明。|
|`300`| [シャッフルシャーディングを使ったワークロードの分離](https://aws.amazon.com/jp/builders-library/workload-isolation-using-shuffle-sharding/)| -| DDoS 攻撃への対処としてのシャッフルシャーディングの解説。|

## S3
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`400`| [Diving Deep on S3 Consistency (English)](https://www.allthingsdistributed.com/2021/04/s3-strong-consistency.html)| -| S3で整合性を保つための仕組みを解説。|
|`---`| [AWS 導入事例：株式会社テレビ東京](https://aws.amazon.com/jp/solutions/case-studies/tv-tokyo/)| -| 13PB のテレビ映像アーカイブを Amazon S3 / S3 Glacier へ移行。|

## Site-to-Site VPN (サイト間 VPN)
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`300`| [[AWS] Site to Site VPN の BGP 経路を制御しよう - DevelopersIO](https://dev.classmethod.jp/articles/control-bgp-route-on-site-to-site-vpn/)| -| Site-to-Site VPN を利用した場合の2つのトンネルと Virtual Private Gateway(VGW), Transit Gateway を利用した場合の BGP による経路制御の方法が分かりやすくまとめっている。|
|`300`| [Simulating Site-to-Site VPN Customer Gateways Using strongSwan - AWSNetworking & Content Delivery](https://aws.amazon.com/blogs/networking-and-content-delivery/simulating-site-to-site-vpn-customer-gateways-strongswan/)| -| AWS 環境のみで擬似的にオンプレミスのネットワークを作成し、Site-toSite VPN を構築する手順。Certificate-based な [part 2](https://aws.amazon.com/blogs/networking-and-content-delivery/simulating-site-to-site-vpn-customer-gateways-using-strongswan-part-2-certificate-based-authentication/)もある。|

## Systems Manager
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [AWS Systems Manager(SSM) の数多い機能群を攻略するための図を書いてみた 2021 - DevelopersIO](https://dev.classmethod.jp/articles/all-ssm-capabilities-2021/)| -| Systems Manager の機能一覧が把握しやすい図。|
|`200`| [AWSでSSMエージェントの自動更新をCloudFormationのスタックセット(StackSets)で複数のリージョンやアカウントに適用](https://zenn.dev/sugikeitter/articles/automating-updates-to-ssm-agent-with-cfn-stacksets)| -| マルチアカウント環境などで全てのサーバーのSSMエージェントの自動更新させる方法。|
|`300`| [AWS IAMの安全な管理方法 · DeNA Engineers' Blog](https://engineer.dena.com/posts/2019.12/aws-iam-management/)| -| IAM ロールが利用できないシステムからAWSサービスへのアクセス時に、定期的にIAMユーザのシークレットアクセスキーのローテートを行う方法。|

## SQS
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| SQS 標準キューのCLIを利用した動作デモ|[`YouTube`](https://www.youtube.com/watch?v=8cAk1_GSV0g&t=336s)| 動画なのでプロデューサー・キュー・コンシューマーの関係がわかりやすい。順序保証がないことや、コンシューマーを増やすことで処理量が線形的に増えていくことがわかる。|
|`200`| SQS FIFOキューのCLIを利用した動作デモ|[`YouTube`](https://www.youtube.com/watch?v=8cAk1_GSV0g&t=660s)| 標準キューと比較してコンシューマーが増えても処理量が線形的に増えるわけではないことや、並列化をしたい場合のグループID利用、プロデューサーからの重複排除が可能なことがわかる。|

## SSO
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [Azure AD と AWS SSOの連携 - fu3ak1's tech days](https://fu3ak1.hatenablog.com/entry/2020/12/20/000622)| -| IdP として Azure Active Directory を利用したAWS SSO の構築方法。|
|`200`| [AWS クラウドサービス活用資料集 - AWSアカウント シングルサインオンの設計と運用 #IDフェデレーションで変わる運⽤の論点](https://d1.awsstatic.com/webinars/jp/pdf/services/20200722_AWSBlackbelt_%E3%82%B7%E3%83%B3%E3%82%B0%E3%83%AB%E3%82%B5%E3%82%A4%E3%83%B3%E3%82%AA%E3%83%B3%E3%81%AE%E8%A8%AD%E8%A8%88%E3%81%A8%E9%81%8B%E7%94%A8.pdf#page=53)| -| 権限セット数に制限がある中で多くのアカウントを管理する場合、 RBAC ではなく ABAC モデルの考え方について。|
|`200`| [AWS SSO、AD、ABACを触ってみる - サーバーワークスエンジニアブログ](https://blog.serverworks.co.jp/2021/04/16/113023)| -| ABAC の設定手順の一例が記載されている。|

## StepFunctions
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`300`| [分散システムにおけるSagaパターンのAWS Step Functions による実装 #AWSDevDay - Speaker Deck](https://speakerdeck.com/fatsushi/fen-san-sisutemuniokerusagapatanfalseaws-step-functions-niyorushi-zhuang-number-awsdevday)| -| Saga パターンについての話と、Step Functions によるエラーハンドリングとリトライ、[e-コマースの注文処理のサンプル実装例](https://github.com/aws-samples/aws-step-functions-long-lived-transactions)など。|

## Transit Gateway
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [クロスアカウントな AWS Transit Gateway を、絵で見て（完全に）理解する。 - DevelopersIO](https://dev.classmethod.jp/articles/transitgateway-cross-account-diagram/)| -| Transit Gateway コンポーネントの位置関係、関連付け（アソシエーション）と伝播（プロパゲーション）が絵でわかりやすい。|

## VPC endpoints (VPCe) / PrivateLink
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [2つのVPCエンドポイントの違いを知る - DevelopersIO](https://dev.classmethod.jp/articles/vpc-endpoint-gateway-type/)| -| ゲートウェイ型とインターフェイス型の2種類の経路違いが図で簡潔にまとめられている。|
|`300`| [「Amazon S3 インターフェースエンドポイント（PrivateLink）ではプライベート DNS をサポートしていません」 の意味を絵をかいて腹落ちさせてみた - DevelopersIO](https://dev.classmethod.jp/articles/s3-privatelink-diagram/)| -| PrivateLink を利用した場合に設定される DNS 名が整理されている。|
|`---`| | [住信SBIネット銀行の PrivateLink 事例](https://pages.awscloud.com/rs/112-TZM-766/images/K1-02.pdf#page=27)| -| 提携企業へ利用してもらうシステムをインターネットに公開することなく PrivateLink を利用することで AWS のネットワークに閉じた形で複数企業へ提供している事例。|

# カテゴリ別

## Availability
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [なぜ「AWS で負荷分散は３AZ にまたがるのがベストプラクティス」と言われるのか 可用性の面から考えてみた](https://dev.classmethod.jp/articles/202008-three-az-load-balancing/)| -| AZ が多い場合のメリットや過去の AZ 障害などの話。|

## Backup / Disaster Recovery
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`300`| [Disaster Recovery of Workloads on AWS: Recovery in the Cloud - Disaster Recovery of Workloads on AWS: Recovery in the Cloud](https://docs.aws.amazon.com/ja_jp/whitepapers/latest/disaster-recovery-workloads-on-aws/disaster-recovery-workloads-on-aws.html)| -| 障害復旧のホワイトペーパー。|

## Cache
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [Webアプリケーションのキャッシュ戦略とそのパターン / Pattern and Strategy of Web Application Caching - Speaker Deck](https://speakerdeck.com/moznion/pattern-and-strategy-of-web-application-caching)| -| キャッシュのメリット・デメリットとデザインパターン。|

## CI / CD
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [GitLab Flow + GitHub Actions ではじめる、デプロイフローの改善・自動化](https://techblog.exawizards.com/entry/2021/01/21/111031)| -| デプロイの課題と GitHub Flow, GitLab Flow について。|
|`200`| [コンテナ Lambda の CI/CD パイプラインを SAM Pipeline で作ろう ! ~コンテナ利用者に捧げる AWS Lambda の新しい開発方式 ! ~ 第 5 回 - builders.flash☆](https://aws.amazon.com/jp/builders-flash/202109/new-lambda-container-development-5/?awsf.filter-name=*all)| -| サーバーレスの CI/CD パイプラインの代表的な構築方法と選択の仕方など。|
|`300`| [安全なハンズオフデプロイメントの自動化](https://aws.amazon.com/jp/builders-library/automating-safe-hands-off-deployments/)| -| Amazon での安全な継続的デプロイメントについて。[継続的デリバリーによる高速化](https://aws.amazon.com/jp/builders-library/going-faster-with-continuous-delivery/)や[デプロイ時におけるロールバックの安全性の確保](https://aws.amazon.com/jp/builders-library/ensuring-rollback-safety-during-deployments/)も参考に。|

## Container
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [スペシャリストから学ぶコンテナ技術 第 1 回 - 変化を求めるデベロッパーを応援するウェブマガジン](https://aws.amazon.com/jp/builders-flash/202104/chat-container-specialist/)| -| そもそもコンテナとは？なぜコンテナか？についての解説。|
|`200`| [スタートアップのためのコンテナ入門 – 導入編 - AWS Startup ブログ](https://aws.amazon.com/jp/blogs/startup/techblog-container-introduction/)| -| コンテナ利用時・検討時によくある誤解やコンテナにすべきかどうかの考え方、コンテナへの移行ステップなど。|
|`200`| [スタートアップのためのコンテナ入門 – AWS Fargate 編 - AWS Startup ブログ](https://aws.amazon.com/jp/blogs/startup/techblog-container-fargate-1/)| -| Amazon ECS を前提に、コンテナ利用時のホストマシンの運用の課題から Fargate のメリットについて。|
|`200`| [スタートアップのためのコンテナ入門 – Kubernetes 編 - AWS Startup ブログ](https://aws.amazon.com/jp/blogs/startup/techblog-container-k8s-1/)| -| Kubernetes を選択すべきかどうかの考え方や、 AWS で Kubernetes を利用する場合のポイントなど。|
|`300`| [コンテナランタイムの仕組みと、Firecracker、gVisor、Unikernelが注目されている理由。 Container Runtime Meetup #2 － Publickey](https://www.publickey1.jp/blog/20/firecrackergvisorunikernel_container_runtime_meetup_2.html)| -| CRI, OCI とは何か？コンテナランタイムの高レベルと低レベルについてなど。|

## Database (DB)
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [社内SQL研修のために作った資料を公開します - 株式会社AI Shift](https://www.ai-shift.co.jp/techblog/1980)| -| SQL や RDB とは？が簡潔にまとめられている。|

## Data Lake / Data Warehouse (DWH)
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [レイクハウスアーキテクチャとは - Amazon Web Services](https://aws.amazon.com/jp/big-data/datalakes-and-analytics/data-lake-house/)| -| レイクハウスアプローチの仕組みや必要になる理由についてなど。|
|`200`| [貯めるだけじゃもったいない！AWS 分析サービスを使ったデータレイクの有効活用 - AWS Summit Online 2021](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-06_AWS_Summit_Online_2021_ANT01.pdf) | [`YouTube`](https://www.youtube.com/watch?v=95P_6_CJeys)| データレイクについての説明や、AWS でデータレイクを活用するときのサービスの紹介。|

## Developing
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [The Twelve-Factor App （日本語訳）](https://12factor.net/ja/)| -| 多種多様なSaaSアプリケーション開発現場での経験と観察をまとめた、ソフトウェア開発の方法論。|
|`200`| [「The Twelve-Factor App」を15項目に見直した「Beyond the Twelve-Factor App」を読んだ - kakakakakku blog](https://kakakakakku.hatenablog.com/entry/2020/03/09/084833)| -| クラウド化が進み技術的な変化も踏まえて「Beyond the Twelve-Factor App」がアップデートされた内容を簡潔にまとめたもの。|
|`300`| [Boto3(AWS SDK for Python)をコードリーディングして仕組みを理解する](https://zenn.dev/sugikeitter/articles/6648845968cec6)| -| Boto3 のクライアント API とリソース API の実装の違い、boto3 の役割と botocore の役割の違いなど。|


## DevOps
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [Amazon S3を開発・運用する方法 - 巨大なマイクロサービスと組織 - AWS Summit Online 2020](https://pages.awscloud.com/rs/112-TZM-766/images/AWS-33_AWS_Summit_Online_2020_STG01.pdf)| [`AWS`](https://resources.awscloud.com/vidyard-all-players/aws-33-aws-summit-online-2020-720p-2)| S3 の開発チームの DevOps の手法や、そのための組織構成など。|

## Infrastructure as Code (IaC)
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [Infrastructure as Codeに関する技術書籍を執筆しました - How elegant the tech world is...!](https://iselegant.hatenablog.com/entry/2021/06/19/231213)| -| CloudFormation, AWS CDK, Terraform, Pulumi のツールが簡潔にまとめらている書籍の紹介。|
|`200`| [Terraform職人再入門2020 - Qiita](https://qiita.com/minamijoyo/items/3a7467f70d145ac03324)| -| Terraform v0.14.2 時点での基礎から。|
|`300`| [Infrastructure as Codeのつらみの原因を探れ　恐怖症による負のサイクルを断ち切る“予測可能性” - ログミーTech](https://logmi.jp/tech/articles/324822)| -| IaC ツールのパターンを分けた考え方。|

## Global Infrastructure / Edge Network
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [AWS を顧客が必要とする場所に延伸する：AWS が提案する新しいハイブリッドの形 - AWS Summit Online 2021](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-16_AWS_Summit_Online_2021_CMP04.pdf) | [`Youtube`](https://www.youtube.com/watch?v=K00ZUUSSNjM)| Amazon Outposts、AWS Local Zones、AWS Wavelength の紹介。|
|`200`| [ユーザーエクスペリエンスとセキュリティを最適化する AWS エッジネットワークサービス - AWS Summit Online 2021](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-33_AWS_Summit_Online_2021_NET02.pdf) | [`Youtube`](https://youtu.be/qFxrmCXm8Vg)| エッジロケーションのサービスのパフォーマンス、セキュリティ、コスト最適化などが簡潔にまとめられている。|
|`300`| [Amazon CloudFront と AWS Global Accelerator を使った AWS Global Network の活用方法 - AWS Summit Tokyo 2020](https://pages.awscloud.com/rs/112-TZM-766/images/AWS-29_AWS_Summit_Online_2020_NET02.pdf)| -| Amazon CloudFront と AWS Global Accelerator の違い、使い分けやエッジロケーションの構成/中⾝について。|
|`---`| [AWS 導入事例：スマートニュース株式会社 - AWS](https://aws.amazon.com/jp/solutions/case-studies/smartnews-2021/)| -| 北米ユーザーの閲覧体験を高めるために、AWS Global Accelerator をはじめとするサービスを活用して、北米の 2 拠点を加えたマルチリージョン構成を実現。|

## Microservices (マイクロサービス)
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [スタートアップのためのマイクロサービス入門 - AWS Startup ブログ](https://aws.amazon.com/jp/blogs/startup/techblog-microservices-introduction/)| -| マイクロサービスとは何か？必要かどうかについての考え方についてなど。`「マイクロサービス」という言葉の功罪` という章以降を一読するのがおすすめ。|

## Migration (マイグレーション・移行)
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [マイグレーションを実現するために - 第 1 回 : 既存システムのマイグレーションはなぜ必要なのか ? - builders.flash☆](https://aws.amazon.com/jp/builders-flash/202010/migration-to-cloud/?awsf.filter-name=*all)| -| クラウドへの移行の必要性や段取りがまとめられている。[第2回](https://aws.amazon.com/jp/builders-flash/202011/migration-to-cloud-2/?awsf.filter-name=*all)、[第3回](https://aws.amazon.com/jp/builders-flash/202102/migration-to-cloud-3/?awsf.filter-name=*all)のシリーズもの。|
|`200`| [Amazon RDS for Oracle / SQL Server への移行ベストプラクティス - AWS Summit 2019](https://pages.awscloud.com/rs/112-TZM-766/images/B3-01.pdf)| -| 考えられる移行パスや、ニアゼロダウンタイム移行の一例など。|
|`200`| [AWSのサービスを使ったオンプレミスからのデータベース移⾏ - AWS Summit Online 2020](https://pages.awscloud.com/rs/112-TZM-766/images/AWS-18_AWS_Summit_Online_2020_DAT01.pdf)| -| データベースを移⾏する際のパターン、SCT/DMSを活⽤したデータベース移⾏の具体例など。|

## Monitoring (モニタリング・監視)
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [AWS Startup Tech Meetup #3: かんたんコンテナロギング選手権](https://speakerdeck.com/prog893/aws-startup-tech-meetup-number-3-kantankontenaroginguxuan-shou-quan)| -| コンテナのログのよくある課題、ログの種類や転送方法、格納先、サンプルアーキテクチャ。|
|`300`| [KubernetesでFluentdの信頼性を担保するための3つの観点](https://zenn.dev/taisho6339/articles/eff38b47cbdbcb)| -| マイクロサービスやコンテナのログでよく利用される Fluentd の信頼性について。|

## Multi Account (マルチアカウント)
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [これが基本のマルチアカウント管理 - AWS Expert Online for JAWS-UG #15](https://www.slideshare.net/AmazonWebServicesJapan/20210526-aws-expert-online) | [`YouTube`](https://www.youtube.com/watch?v=3QJ-RA5R0Jk)| マルチアカウント管理の必要性や考え方、ベストプラクティス、Control Tower による LandingZone の実現、具体的なガードレールの実装。アカウント分割により管理できる例が[ここ](https://www.slideshare.net/AmazonWebServicesJapan/20210526-aws-expert-online/7)や[Landing Zone とは](https://www.slideshare.net/AmazonWebServicesJapan/20210526-aws-expert-online/26)の説明がわかりやすい。|
|`200`| [「AWS Control Towerを利用したマルチアカウント管理とセキュリティ統制」JAWS DAYS 2021登壇資料 #jawsug #jawsdays #jawsdays2021 #jawsdays2021_C - DevelopersIO](https://dev.classmethod.jp/articles/jaws-days-2021-control-tower/)| [`YouTube`](https://youtu.be/JpJjJ39c5oQ)| [ここ](https://speakerdeck.com/cmusudakeisuke/aws-control-towerwoli-yong-sitamarutiakauntoguan-li-tosekiyuriteitong-zhi?slide=10)からのアカウントを分けることによる分離の考え方の図がわかりやすい。|
|`200`| [やらないという選択肢はない　AWS Configを用いたマルチアカウント・マルチリージョンでのリソース把握とコンプライアンス維持 - ログミーTech](https://logmi.jp/tech/articles/323894)| -| AWS Configを用いたマルチアカウント・マルチリージョンでのリソース把握とコンプライアンス維持への取り組み|
|`200`| [AWS Organizationsを活用したマルチアカウントのセキュリティサービス使用方法 ～まとめ～ - fu3ak1's tech days](https://fu3ak1.hatenablog.com/entry/2021/01/28/002536)| -| Organizationsを活用したセキュリティサービスについての紹介。|
|`200`| [「進化し続けるインフラ」でありたい　リクルートのAWS基盤チームによるマルチアカウント管理 - ログミーTech](https://logmi.jp/tech/articles/323814)| -| 約90の AWS アカウントに対して横断的な管理、コスト配賦、共通機能の提供などの運用について。|
|`300`| [AWS Organizations における組織単位のベストプラクティス - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/best-practices-for-organizational-units-with-aws-organizations/)| -| AWS が推奨する「ランディングゾーン」と呼ばれる安全かつ生産性の高いマルチアカウント AWS 環境を構築する要素について。組織単位 (Organization Unit: OU) の分割方法など。|

## Multi Region (マルチリージョン)
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [マルチリージョン、ちょっとその前に...-サービスの可用性について考える - AWS Summit Online 2021](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-53_AWS_Summit_Online_2021_Thinking-about-Availability.pdf) | [`Youtube`](https://www.youtube.com/watch?v=8MyZ84WEjrc)| マルチリージョン構成でのデータ整合性や切替⽅式などの重要な検討事項、ビジネスニーズとコストのバランスについて。|
|`200`| [Network視点で考えるシームレスなマルチリージョンへの移行と検討](https://pages.awscloud.com/rs/112-TZM-766/images/ORL-T3-Session.pdf)| -| マルチリージョン構成で Route53, Global Accelerator の違いなど。|

## Network
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [AWS Summit Tokyo 2019 - 【初級】AWS を支えるグローバルネットワーク](https://pages.awscloud.com/rs/112-TZM-766/images/C1-02.pdf)| -| AWS のデータセンターやネットワークの物理構成と特徴やメリットについて。|
|`300`| [AWSネットワークの論理的な側面 ～ AWSのバックボーンネットワークに関するDeepな話（2） (1/4)：CodeZine（コードジン）](https://codezine.jp/article/detail/9790)| -| Mapping Service (マッピングサービス)を利用した VPC 内で仮想サーバー同士が通信可能な仕組みの解説。|
|`300`| [パケットの気持ちになって辿る Amazon VPC のルーティング - AWS Summit Online 2020](https://pages.awscloud.com/rs/112-TZM-766/images/AWS-08_AWS_Summit_Online_2020_NET01.pdf)| -| オンプレミスのルーター/スイッチの考え方とは異なる、VPC 内でのクラウドネットワーキングの感覚を掴む。|
|`300`| [「知らなくても困らないけど、知ると楽しいVPCの裏側の世界」というテーマでビデオセッションでお話ししました #devio2020 - DevelopersIO](https://dev.classmethod.jp/articles/devio-connect-2020-chibayuki-vpc/)| -| AWS Hyperplane や Blackfoot という VPC を裏側で支える技術について。 |
|`300`| [顧客拠点から Amazon VPCへの接続パターンまとめ (Whitepaper参照） - DevelopersIO](https://dev.classmethod.jp/articles/whitepaper-translate-jpn-vpc-connectivity-options-01/)| -| VGW, Direct Connect, Transit Gateway の利用パターンがまとまっている。|

## Security
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [AWS セキュリティ監査のガイドライン - AWS 全般のリファレンス](https://docs.aws.amazon.com/ja_jp/general/latest/gr/aws-security-audit-guide.html)| -| 基本的なことではあるが、監査を実践するためのガイドラインが羅列されている。|
|`200`| [AWSの異常課金で気付いた不正アクセス--インシデントにどう対応したのか - ZDNet Japan](https://japan.zdnet.com/article/35133681/)| -| 初動対応の調査や、社内の対応体制と外部連携についてなど。|
|`200`| [ゼロトラストアーキテクチャ: AWS の視点 - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/zero-trust-architectures-an-aws-perspective/)| -| ゼロトラストの定義と指針など。|
|`200`| [AWS 環境における脅威検知と対応 - AWS Summit Online 2021](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-39_AWS_Summit_Online_2021_SEC03.pdf)| -| Amazon GuardDuty、AWS Security Hub、Amazon Detective による脅威を検知、監視、調査について。|
|`300`| [AWS環境にセキュアなベースラインを提供するテンプレート「Baseline Environment on AWS」のご紹介 - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/announcing-baseline-environment-on-aws/)| -| AWS Japanのソリューションアーキテクトが AWS Samples に公開している BLEA についての紹介。Control Tower によるマルチアカウント環境でも同じように利用可能。|
|`300`| [2020年版 チーム内勉強会資料その1 : JSON Web Token - r-weblife](https://ritou.hatenablog.com/entry/2020/06/08/050000)| -| Cognito でも利用されている JSON Web Token(JWT) について。|

## Serverless (サーバーレス)
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [形で考えるサーバーレス設計 / サーバーレスパターン - AWS](https://aws.amazon.com/jp/serverless/patterns/serverless-pattern/)| -| サーバーレスの組み合わせの代表的な適用シーン/ユースケースと実装形。|
|`300`| [イチから理解するサーバーレスアプリケーション - 開発サーバーレス開発環境とテスト](https://pages.awscloud.com/rs/112-TZM-766/images/20200827_serverless_session2.pdf)| -| [テストしやすい Lambda 関数の書き方](https://pages.awscloud.com/rs/112-TZM-766/images/20200827_serverless_session2.pdf#page=56)や、[AWSのサービスを利⽤するコードのUnit Test](https://pages.awscloud.com/rs/112-TZM-766/images/20200827_serverless_session2.pdf#page=73)の方法論など。|
|`300`| [2021年版、サーバーレスのテスト手法を考える / Serverless Testing 2021 - Speaker Deck](https://speakerdeck.com/_kensh/serverless-testing-2021)| -| 外部リソースを含むテスト、後半なスタックで構成されたビジネスロジック、非同期の副作用を伴うテストなど。|
|`300`| [今日から始める、サーバーレス Well-Architected Framework - Speaker Deck](https://speakerdeck.com/_kensh/serverless-well-architected-framework)| -| Well-Architected フレームワークに則った設計をするための具体例。|
|`300`| [Serverless Land - Resources for learning about AWS serverless technology](https://serverlessland.com/)| -| サーバーレスの設計パターンなど。|

## Storage
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [ストレージの勉強方法を聞いてみた。 - 変化を求めるデベロッパーを応援するウェブマガジン](https://aws.amazon.com/jp/builders-flash/202110/way-to-learn-storage/)| -| おすすめの資料や書籍なども。|
|`200`| [Comparing your on-premises storage patterns with AWS Storage services - AWS Storage Blog (English)](https://aws.amazon.com/blogs/storage/comparing-your-on-premises-storage-patterns-with-aws-storage-services/)| -| オンプレミスのストレージの考え方と、 AWS でのストレージの考え方。|
|`200`| AWS Storage - EBS vs S3 vs EFS| [`YouTube`](https://www.youtube.com/watch?v=6vNC_BCqFmI)| [ここから](https://youtu.be/6vNC_BCqFmI?t=238) EBS, S3, EFS の違いがわかりやすく解説されている。|
