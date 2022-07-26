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
|[AWS グローバルインフラストラクチャ](https://aws.amazon.com/jp/about-aws/global-infrastructure/)| AWS グローバルインフラストラクチャの最新情報やメリットなど。[AWS のデータセンターのページ](https://aws.amazon.com/jp/compliance/data-center/data-centers/)や、エッジロケーションの位置が記載された [CloudFront の特徴](https://aws.amazon.com/jp/cloudfront/features/)のページも用意されている。3分弱の動画である [AWS データセンターのセキュアな設計について - YouTube](https://www.youtube.com/watch?v=1-Bbe9_7J4o) もおすすめ。|
|[サービスエンドポイントとクォータ - AWS 全般のリファレンス](https://docs.aws.amazon.com/ja_jp/general/latest/gr/aws-service-information.html)| AWS サービスごとの API を利用する際の URL の一覧。 [サービス別の FIPS エンドポイント](https://aws.amazon.com/jp/compliance/fips/) の一覧もある。|
|[AWS API リクエストの署名 - AWS 全般のリファレンス](https://docs.aws.amazon.com/ja_jp/general/latest/gr/signing_aws_api_requests.html)| AWS の API をリクエストするために必要な署名バージョン 4 の [署名プロセス](https://docs.aws.amazon.com/ja_jp/general/latest/gr/signature-version-4.html)、[リクエスト要素](https://docs.aws.amazon.com/ja_jp/general/latest/gr/sigv4_elements.html)、[署名の作成手順](https://docs.aws.amazon.com/ja_jp/general/latest/gr/sigv4_signing.html)など。|
|[AWS Well-Architected のポータルサイト](https://aws.amazon.com/jp/architecture/well-architected/)| AWS Well-Architected フレームワーク、レンズ、Tool などの情報がまとめられている。|
|[What’s New at AWS (English)](https://aws.amazon.com/new/)| AWS の最新リリース情報が更新れている。[日本語版はこちら](https://aws.amazon.com/jp/new/)。|
|[よくある質問](https://aws.amazon.com/jp/faqs/)| サービスごとによくある質問ページが用意されていて、利用する時に知りたい情報が多く書かれている |
|[AWS サポート - ナレッジセンター](https://aws.amazon.com/jp/premiumsupport/knowledge-center/)| AWS のお客様から最も頻繁に寄せられるご質問とご要望をいくつかご紹介しているサイト。|
|[AWSサービス別資料](https://aws.amazon.com/jp/aws-jp-introduction/aws-jp-webinar-service-cut/)| 各サービスごとに基礎から発展的な知識まで素早く知るのに役立つ資料集|
|[AWS 料金見積りツール - AWS Pricing Calculator](https://calculator.aws/#/)| サービスごとのコスト見積もりができるツール。料金表自体は各サービスの料金ページに記載がある。|

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
|[AWS Prescriptive Guidance](https://aws.amazon.com/prescriptive-guidance/)| クラウドの移行、モダナイゼーション、プロジェクトの最適化を促進するのに役立つ、実績のある戦略やガイド、パターンを提供する規範的ガイダンス。|

## AWS 関連の GitHub リポジトリ
|URL|備考|
|---|---|
|https://github.com/aws| AWS の CLI, SDK, CDK, SAM などの OSS ツールなど。|
|https://github.com/awslabs| ↑以外の AWS の OSS ツールなど。|
|https://github.com/awsdocs| ユーザーガイドなどのドキュメントや [SDK のサンプルコード](https://github.com/awsdocs/aws-doc-sdk-examples)など。|
|https://github.com/aws-samples| AWS の利用例やワークショップなど。 |
|https://github.com/aws-ia| AWS Integration and Automation のリポジトリ。Terraform に関するものが多いが、CloudFormation 関連のものも少しある。|
|https://github.com/boto| AWS CLI のコアロジックや AWS SDK for Python のコード。|
|https://github.com/aws-amplify| AWS Amplify の独立したリポジトリ。|
|https://github.com/aws-containers| AWS コンテナ関連の独立したリポジトリ。ツールや利用例、ワークショップなど。|

## AWS SDK ドキュメント
|URL|備考|
|---|---|
| [AWS SDK for .NET V3 API](https://docs.aws.amazon.com/sdkfornet/v3/apidocs/index.html)| シンプルな API ドキュメント。|
| [AWS SDK for Java](https://sdk.amazonaws.com/java/api/latest/)| javadoc を HTML にした Java ユーザーにはお馴染みの形式。|
| [AWS SDK for Python (Boto3)](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html)| 1ページの情報量が多いので、少し表示が重いこともあるので注意。|

## 学習に役立つ情報
|URL|備考|
|---|---|
|[ハンズオンの「腹落ち問題」を改善する 5 Tips - builders.flash☆](https://aws.amazon.com/jp/builders-flash/202103/five-tips-accept-handson-situation/)| ハンズオンや演習を手順通り実施した時の学習効果をより高めるための Tips が紹介されている。とても納得感がありおすすめ！|
|[AWS のアーキテクチャ図を描きたい ! でもどうすれば良いの ? - builders.flash☆](https://aws.amazon.com/jp/builders-flash/202204/way-to-draw-architecture/)| AWS のアーキテクチャ図を描くときに最初に読んでおくと効果的な内容。|
|[AWS Stash](https://awsstash.com/)|公式ではないがAWS関連資料が高速に検索できるサイト。|
| `site:d1.awsstatic.com`<br>`site:pages.awscloud.com`| Google 検索のキーワードに追加すると、AWS イベントの発表資料の PDF が多く検索結果にヒットするので便利。`site:d0.awsstatic.com`もあるけど少し古め？かも。両方のドメインをまとめて検索したい場合は`<検索ワード> site:pages.awscloud.com OR site:d1.awsstatic.com`で検索可能。|

## 初めてアカウントを作る方へ
|URL|備考|
|---|---|
|[AWS アカウント作成の流れ - AWS](https://aws.amazon.com/jp/register-flow/)| キャプチャ付きの AWS アカウント作成フロー。|
|[AWSアカウントを作ったら最初にやるべきこと 〜2021年版〜 #devio2021  DevelopersIO](https://dev.classmethod.jp/articles/aws-1st-step-2021/)| |
|[AWSアカウント作成時にやるべきこと - NRIネットコムBlog](https://tech.nri-net.com/entry/aws_first_security)| |

# サービス別

## API Gateway
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`300`| [Amazon API Gateway は何をしてるのか - DevelopersIO](https://dev.classmethod.jp/articles/what-does-amazon-api-gateway-do/)| -| API Gateway の機能が網羅的に纏まっている。|


## App Runner
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| AWS App Runner とは？ - AWS Expert Online for JAWS-UG #16| [`YouTube`](https://www.youtube.com/watch?v=--o2HwfnFiY)| App Runner の使い方とメリットを、デモを通して紹介。|

## CDK
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`300`| [AWS CDKでクラウドアプリケーションを開発するためのベストプラクティス - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/best-practices-for-developing-cloud-applications-with-aws-cdk/)| -| |

## Client VPN
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [ノマド・ワーカーのためのVPNクライアント設定入門：運用（1/5 ページ） - ＠IT](https://atmarkit.itmedia.co.jp/ait/articles/1302/27/news016.html)| -| インターネットを利用した クライアント端末との VPN についてのわかりやすい絵が記載されている。|
|`200`| [AWS Client VPN のリソースとパラメータを一枚絵にまとめつつ過去のエントリもまとめてみた - DevelopersIO](https://dev.classmethod.jp/articles/aws-client-vpn-perfect-understand-2/)| -| 証明書や認証周りなども含めて整理されている。|
|`---`| [AWS 導入事例：コクヨ株式会社 - AWS](https://aws.amazon.com/jp/solutions/case-studies/kokuyo-serverworks/)| -| Direct Connect は利用している状態から、1,000 名規模のリモートワーク環境を10日間で構築した話。|
|`---`| [AWS を使って安全で快適なリモートワーク環境を導入したお話(後編)](https://tech.bitbank.cc/20201212/)| -| 自社で VPN の運用をする場合に大変だった点と AWS の VPN 利用でのメリット。|


## CloudFormation
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [AWS Organizations × CloudFormation StackSetsの組み合わせが素晴らしい - プログラマでありたい](https://blog.takuros.net/entry/2020/03/25/093247)| -| StackSets の利用例とメリットなど。|
|`---`| [AWS 導入事例：本田技研工業株式会社 - AWS](https://aws.amazon.com/jp/solutions/case-studies/honda/)| -| CloudFormation の活用でサーバー環境の設定を差分なく各リージョンに展開することができ、通常なら1拠点で2～3ヶ月はかかるところを、約2週間に短縮。|
|`---`| [AWS 導入事例：京セラ株式会社 - AWS](https://aws.amazon.com/jp/solutions/case-studies/kyocera/)| -| 開発、検証、本番の3つの環境を合わせて数百台のサーバーを用意する必要があり、テンプレートを使って環境を自動構築する CloudFormation などを利用して工数を削減。|


## CloudFront
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [CloudFront Functions の導入 – 任意の規模において低レイテンシーでコードをエッジで実行 - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/introducing-cloudfront-functions-run-your-code-at-the-edge-with-low-latency-at-any-scale/)| -| CloudFront Functions のユースケースと Lambda@Edge との比較など。|
|`300`| [Visitor PrioritizationソリューションをCloudFront Functionsを使って実装するための考慮点 - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/visitor-prioritization-by-cloudfront-functions/)| -| CloudFront Functions を利用したユーザーの優先制御、流量制御を行うための静的なウェイティングルームページにに誘導するソリューション。|

## CloudHSM
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`---`| [AWSセキュリティ事例 -  ITソリューションのTIS株式会社](https://www.tis.jp/special/aws_security/)| -| 株式会社日本カードネットワークが決済ネットワークの J-Helix システムで、取り扱うデータの暗号化と暗号鍵の管理に CloudHSM と KMS を利用した事例。|

## CloudTrail
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [AWS CloudTrail ログをモニタリングするためのベストプラクティス - Datadog](https://www.datadoghq.com/ja/blog/monitoring-cloudtrail-logs/)| -| AWS CloudTrail 監査ログの構造、監視する重要な CloudTrail ログ、Datadog との連携など。|

## CodeCommit
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [awslabs/git-secrets: Prevents you from committing secrets and credentials into git repositories](https://github.com/awslabs/git-secrets)| -| 認証情報を Git でコミットさせないためのツール。|

## Cognito
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [アプリにユーザー認証機能を簡単に追加 !「Amazon Cognito」をグラレコで解説 - builders.flash](https://aws.amazon.com/jp/builders-flash/202103/awsgeek-cognito/)| -| Cognito の概要がわかりやすい絵と共に解説されている。|
|`200`| [AWS再入門ブログリレー Amazon Cognito編 - DevelopersIO](https://dev.classmethod.jp/articles/re-introduction-2020-amazon-cognito/)| -| ユーザープール、ID プールの利用パターンが解説されている。|
|`200`| [Cognitoのサインイン時に取得できる、IDトークン・アクセストークン・更新トークンを理解する - DevelopersIO](https://dev.classmethod.jp/articles/study-tokens-of-cognito-user-pools/)| -| Cognito で利用するトークンの解説。|

## Config
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [AWS Config ベストプラクティス - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/aws-config-best-practices/)| -| Config を利用する場合に確認しておきたい20の項目。「1 つのリージョンでのみグローバルリソース (IAM リソースなど) を記録」など。|

## Control Tower
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [AWS ソリューションプロバイダー向け AWS Control Tower のベストプラクティス - AWS JAPAN APN ブログ](https://aws.amazon.com/jp/blogs/psa/aws-control-tower-best-practices-for-aws-solution-providers/)| -| ソリューションプロバイダープログラムのお客様が AWS Control Tower を導入から継続的な運用までのプロセスを機能させる方法。|
|`200`| [AWS Control Towerの嬉しいポイントと注意ポイント - NRIネットコム Design and Tech Blog](https://tech.nri-net.com/entry/controltower-kms)| -| AWS Control Tower を実際に利用するときのポイント。|
|`300`| [Customize your AWS Control Tower landing zone - AWS Control Tower](https://docs.aws.amazon.com/controltower/latest/userguide/customize-landing-zone.html)| -| [Customizations for AWS Control Tower (CfCT)](https://docs.aws.amazon.com/controltower/latest/userguide/cfct-overview.html) と呼ばれる Control Tower のカスタマイズ方法の実装の一例などを紹介。[CfCT のブログ](https://aws.amazon.com/jp/blogs/architecture/fast-and-secure-account-governance-with-customizations-for-aws-control-tower/) や [CfCT のデプロイ手順動画 (YouTube)](https://www.youtube.com/watch?v=JZPxHW9pjsA)、[AWS re:Invent 2021 - Customizing and scaling your AWS Control Tower environment (YouTube)](https://www.youtube.com/watch?v=fDtxiBW_J8I)、[日本語の Workshop](https://controltower.aws-management.tools/ja/automation/cfct/) も参考に。|
|`300`| [「AWS Control Tower をカスタマイズして使ってみよう」というテーマでお話ししました #devio2021 - DevelopersIO](https://dev.classmethod.jp/articles/devio2021-cfcf/)|[`YouTube`](https://www.youtube.com/watch?v=j-7hN8te0Yo)| Control Tower でセットアップされないけれど初期設定に組み込みたいサービスのカスタマイズ方法の一例。|

## Direct Connect (DX)
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [パートナー - AWS Direct Connect](https://aws.amazon.com/jp/directconnect/partners/)| -| DX ロケーションとパートナーの一覧。|
|`300`| [AWS Direct Connect でのアクティブ/パッシブ BGP 接続の構築 - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/creating-active-passive-bgp-connections-over-aws-direct-connect/)| -| 複数の DX 接続を利用して、経路制御やネットワークの最適化をする方法。|
|`---`| [AWS導入事例 株式会社ゼンリンデータコム様 - TOKAIコミュニケーションズ AWSソリューション](https://www.cloudsolution.tokai-com.co.jp/case/zenrin-datacom.html)| -| お客様データセンター <-> DXロケーション <-> AWS のネットワークへの接続の具体的な図がわかりやすい。|

## DMS
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [はじめてAWS DMSを検討する際に読んでいただきたいこと - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/first-step-of-dms/)| -| AWS DMSの特徴と強みや、物理レプリケーション方式と論理（ロジカル）レプリケーション方式の違い、利用する際の注意点がまとまっている。|

## DynamoDB
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| Amazon DynamoDB Deep Dive - AWS Summit Tokyo 2019|[`YouTube`](https://www.youtube.com/watch?v=16RYHfe89WY)| DynamoDB の基本から内部構造の詳細、デザインパターンなどの発展的な情報まで。|
|`200`| [OPENREC.tv における Amazon DynamoDB を用いた スケーラブルなアプリケーション設計 - CyberZ, Inc.](https://pages.awscloud.com/rs/112-TZM-766/images/Session%204%20-%2020200825_CyberZ_OPENRECTV_Purpose-Built-Databases-Week-v2.pdf)| -| [プロビジョンド / オンデマンドのユースケース](https://pages.awscloud.com/rs/112-TZM-766/images/Session%204%20-%2020200825_CyberZ_OPENRECTV_Purpose-Built-Databases-Week-v2.pdf#page=27)がわかりやすい。|
|`300`| [サーバーレスアプリケーション向きの DB 設計ベストプラクティス](https://pages.awscloud.com/rs/112-TZM-766/images/20190905_%E3%82%A4%E3%83%81%E3%81%8B%E3%82%89%E7%90%86%E8%A7%A3%E3%81%99%E3%82%8B%E3%82%B5%E3%83%BC%E3%83%8F%E3%82%99%E3%83%BC%E3%83%AC%E3%82%B9%E3%82%A2%E3%83%95%E3%82%9A%E3%83%AA%E9%96%8B%E7%99%BA-%E3%82%B5%E3%83%BC%E3%83%8F%E3%82%99%E3%83%BC%E3%83%AC%E3%82%B9%E3%82%A2%E3%83%95%E3%82%9A%E3%83%AA%E3%82%B1%E3%83%BC%E3%82%B7%E3%83%A7%E3%83%B3%E5%90%91%E3%81%8D%E3%81%AEDB%20%E8%A8%AD%E8%A8%88%E3%83%98%E3%82%99%E3%82%B9%E3%83%88%E3%83%95%E3%82%9A%E3%83%A9%E3%82%AF%E3%83%86%E3%82%A3%E3%82%B9.pdf)| -| 2019/09/05 に開催された AWS のイベント、「イチから理解するサーバーレスアプリ開発」における講演資料の一つ。[p.18](https://pages.awscloud.com/rs/112-TZM-766/images/20190905_%E3%82%A4%E3%83%81%E3%81%8B%E3%82%89%E7%90%86%E8%A7%A3%E3%81%99%E3%82%8B%E3%82%B5%E3%83%BC%E3%83%8F%E3%82%99%E3%83%BC%E3%83%AC%E3%82%B9%E3%82%A2%E3%83%95%E3%82%9A%E3%83%AA%E9%96%8B%E7%99%BA-%E3%82%B5%E3%83%BC%E3%83%8F%E3%82%99%E3%83%BC%E3%83%AC%E3%82%B9%E3%82%A2%E3%83%95%E3%82%9A%E3%83%AA%E3%82%B1%E3%83%BC%E3%82%B7%E3%83%A7%E3%83%B3%E5%90%91%E3%81%8D%E3%81%AEDB%20%E8%A8%AD%E8%A8%88%E3%83%98%E3%82%99%E3%82%B9%E3%83%88%E3%83%95%E3%82%9A%E3%83%A9%E3%82%AF%E3%83%86%E3%82%A3%E3%82%B9.pdf#page=18) から RDB と DynamoDB のデータベース設計プロセスの違いが記載されている。|
|`300`| [Amazon DynamoDB deep dive: Advanced design patterns](https://pages.awscloud.com/rs/112-TZM-766/images/Session%203%20-%20purpose_built_database_DynamoDB_advancedDP_narita_rev.pdf) | -| NoSQL の正規化と非正規化によるデータモデリング / 複合key、階層的構造のデータ、リレーショナルなデータの表現などのデザインパターン / 実際のアプリケーションにおけるモデリング など。|
|`300`| [DynamoDB Immersion Days 参加レポート - ZOZO TECH BLOG](https://techblog.zozo.com/entry/dynamodb-immersion-days)| -| DynamoDB の機能を有効に使うためのデザインパターンがわかりやすくレポートされている。|
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
|`100`| [Amazon EC2 だけじゃない！最⾼のコスト効率を⼿に⼊れるための スポットインスタンス使いこなし術 - AWS Summit Online 2020](https://pages.awscloud.com/rs/112-TZM-766/images/AWS-27_AWS_Summit_Online_2020_CMP01.pdf)| -|[空きキャパシティとスポット価格についてのわかりやすい図](https://pages.awscloud.com/rs/112-TZM-766/images/AWS-27_AWS_Summit_Online_2020_CMP01.pdf#page=14)が記載されている。|
|`200`| [Amazon EC2 の進化の歴史から学ぶ EC2 入門 2019年版 - AWS Summit Tokyo 2019](https://pages.awscloud.com/rs/112-TZM-766/images/C2-06.pdf)|[`YouTube`](https://ww.youtube.com/watch?v=SbKLo5atgk4)| EC2 のインスタンスタイプや機能を時系列に紹介している。|
|`200`| [Amazon EC2インスタンスタイプの選び方ガイド - AWS Summit Tokyo 2019](https://pages.awscloud.com/rs/112-TZM-766/images/C2-07.pdf)|[`YouTube`](https://www.youtue.com/watch?v=Q1LUX8WMjHY)| [EC2 インスタンスのネーミングポリシー](https://pages.awscloud.com/rs/112-TZM-766/images/C2-07.pdf#page=14)と[追加機能のオプション表記](https://pages.awscloud.com/rs/112-TZM-766/images/C2-07.pdf#page=20)がわかりやすい。|
|`200`| [Amazon EC2 ことはじめ 〜あらゆるワークロードに対応する豊富な選択肢とコスト最適化オプション〜 - AWS Summit Online 2021](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-13_AWS_Summit_Online_2021_CMP01.pdf)|[`YouTube`](https://youtu.be/wD-KOWEmx5E)| [EC2インスタンスの選び方](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-13_AWS_Summit_Online_2021_CMP01.pdf#page=12)や、コストとキャパシティーの最適化など。[Savings Plans](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-13_AWS_Summit_Online_2021_CMP01.pdf#page=30)の解説図や[Savings Plans と RI の関係](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-13_AWS_Summit_Online_2021_CMP01.pdf#page=34)がわかりやすい。|
|`300`| [[待望のアプデ]EC2インスタンスメタデータサービスv2がリリースされてSSRF脆弱性等への攻撃に対するセキュリティが強化されました！ - DevelopersIO](https://dev.classmethod.jp/articles/ec2-imdsv2-release/)| -| 開発者の設定不備でインスタンスメタデータサービス(IMDS)から取得できる IAM ロールの一時的なクレデンシャル情報を奪われ、悪用された事例と IMDSv2による改善点など。|
|`---`| [AWS 導入事例：株式会社ゲームフリーク](https://aws.amazon.com/jp/solutions/case-studies/gamefreak/)| -| "最新のゲーム機やゲームシステムの進化は著しく、ゲーム開発の大規模化が進んでいます。そのため、オンプレミスシステムのリソース不足に悩まされるケースも増えていました。それゆえに、開発環境のメンテナンスなどの運用負荷が大きく影響してしまうという課題を抱えていました。「データセンターのリソースにも限りがあり、ラックスペースや電力の不足も大きな問題でした。特にコロナ禍以降はシステムを増強したくとも、マシンを調達することすら困難です。少人数でも運用でき、物理的制限が小さく、環境変化へ柔軟に対応できるスケーラビリティの高いインフラが必要でした」" という部分に AWS 利用のメリットが詰まっている。|
|`---`| [AWS 導入事例：スマートニュース株式会社](https://aws.amazon.com/jp/solutions/case-studies/smartnews/)| -| 朝、昼、夕方、夜と、1日4回のプッシュ通知で訪れるピークを Amazon EC2 Auto Scaling で対応。|
|`---`| [囲碁AIブームに乗って、若手棋士の間で「AWS」が大流行　その理由とは？：週末エンプラこぼれ話（1/4 ページ） - ITmedia エンタープライズ](https://www.itmedia.co.jp/enterprise/articles/1902/22/news006.html)| -| スポットインスタンスを利用して、個人で月に数千〜一万円程で高性能な GPU を搭載したマシンで囲碁AIを導入した話。|
|`---`| [株式会社ディー・エヌ・エー様におけるEC2スポットインスタンスの大規模活用のための工夫とコンテナ技術を用いた設計例の紹介 - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/how-dena-succesfully-applied-ec2-spot-on-production-and-reference-architecture-using-containers/)| -| スポットインスタンスを活用し、最終的に全体のインフラコストを60%削減することに成功した事例。|

## ECS
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [名刺データ化システムをECSに移行した - Sansan Builders Blog](https://buildersbox.corp-sansan.com/entry/2020/12/02/110000)| -| ECS or EKS , Fargate or EC2 の選定理由がわかりやすく記載されている。具体的なデプロイフローもあってすごく良い。|
|`200`| [Pairs, Pairsエンゲージにおける ECS Fargate の移行・活用事例 - 株式会社エウレカ](https://pages.awscloud.com/rs/112-TZM-766/images/04_%E3%82%A8%E3%82%A6%E3%83%AC%E3%82%AB%E6%A7%98_%E8%B3%87%E6%96%99.pdf)| -| コンテナによって開発課題をどう解決したかと ECS on Fargate の採用理由についてなど。[コンテナ移行前のアーキテクチャ図](https://pages.awscloud.com/rs/112-TZM-766/images/04_%E3%82%A8%E3%82%A6%E3%83%AC%E3%82%AB%E6%A7%98_%E8%B3%87%E6%96%99.pdf#page=8)もかなり書き込まれていて面白い。|
|`300`| [第2回 AWS Fargate かんたんデプロイ選手権 #AWSDevDay / The Easiest Deployment Championship 2020 - Find your winner for AWS Fargate! - Speaker Deck](https://speakerdeck.com/toricls/the-easiest-deployment-championship-2020-find-your-winner-for-aws-fargate)| -| ECS のデプロイツール (CloudFormation, Terraform, Copilot, CDK, ecspresso) 比較でそれぞれの Pros/Cons がまとまっている。|
|`---`| [金融スタートアップにおけるコンテナ・ECSの活用事例 / container-fest-summer-fintech - Speaker Deck](https://speakerdeck.com/stajima/container-fest-summer-fintech)| -| コンテナを採用している理由、EKS ではなく ECS を選んだ理由も記載されている。|
|`---`| [【事例】ロマサガRSの大規模トラフィックを捌くAmazon ECS & Docker 運用 - AWS Summit Tokyo 2019](https://pages.awscloud.com/rs/112-TZM-766/images/I3-04.pdf#page=15)| [`YouTube`](https://www.youtube.com/watch?v=SdtbNYP8UH4)| 大規模なゲームを ALB + ECS + RDS + ElastiCache + DynamoDB で構築していて、お手本のようなアーキテクチャ図で参考になる。|

## EKS
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [リクルートマーケティングパートナーズにおけるAmazon EKSとAWS App Meshを使った基盤安定性向上とGitOpsへの挑戦 - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/migration-journey-of-container-orchestrator-by-recruit-marketing-partners/)| -| なぜ ECS から EKS に移行したのかについても記載されている。|
|`200`| [アソビュー！がECSではなくEKSを選んだ理由 - Speaker Deck](https://speakerdeck.com/kirimaru/asobiyu-gaecsdehanakuekswoxuan-ndali-you)| -| どちらが優れているかではない上で、なぜ今回 EKS にしたのかを大変な面も踏まえて「誰が」「何に対して」の観点でまとめられている。|
|`300`| [EKS Anywhereのファーストインプレッション - inductor's blog](https://blog.inductor.me/entry/2021/09/10/031541)| -| |
|`---`| [AWS 導入事例：freee株式会社 - AWS](https://aws.amazon.com/jp/solutions/case-studies/freee/)| -| EKS 利用により Kubernetes のコントロールプレーンの運用を AWS に任せることで開発の課題に対応。|

## ElastiCache
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`---`| [Backends For Frontends（BFF）はじめました - ZOZO TECH BLOG](https://techblog.zozo.com/entry/zozo-aggregation-api-bff)| -| APIと各バックエンドの間に ElastiCache による Redis を利用する事で各モジュールをキャッシュする仕組みを構築。|

## ELB
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`300`| [Network Load BalancerのターゲットグループにApplication Load Balancerを設定する - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/application-load-balancer-aws-privatelink-static-ip-addresses-network-load-balancer/)| -| ALB に固定 IP を設定したい場合の NLB + ALB 構成とユースケースについて。|

## GuardDuty
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [ぎりぎり 20 分で話しきる Amazon GuardDuty による脅威検知](https://pages.awscloud.com/rs/112-TZM-766/images/20220428_17th_ISV_DiveDeepSeminar_Guard_Duty.pdf)| [`Vidyard`](https://play.vidyard.com/JhTTR1GGHgstRkAg5ENhd2)| [【開催報告】アップデート紹介とちょっぴり DiveDeep する AWS の時間 第十七回 (04/28) - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/update-divedeep-series-17/) のセッション。2022年4月時点の GuardDuty の最新情報込みで基本情報がまとめられている。|
|`300`| [Enabling Amazon GuardDuty in AWS Control Tower using Delegated Administrator - AWS Cloud Operations & Migrations Blog (English)](https://aws.amazon.com/jp/blogs/mt/automating-amazon-guardduty-deployment-in-aws-control-tower/)| -| Organizations で管理するアカウントに GuardDuty の設定を適用するソリューションの紹介。Control Tower で作成される Audit アカウントを GuardDuty の管理者アカウントに委譲し、Log Archive アカウントの S3 バケットにログを集約させるための CloudFormation テンプレートが用意されている。|

## IAM
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [IAM JSON ポリシー要素のリファレンス - AWS Identity and Access Management](https://docs.aws.amazon.com/ja_jp/IAM/latest/UserGuide/reference_policies_elements.html)| -| ポリシーに記載できる Statement や Principal, Condition などの要素一覧と、それぞれの要素がどのような構文で記載するかがわかるドキュメント。|
|`100`| [AWS のサービスのアクション、リソース、および条件キー - サービス認証リファレンス](https://docs.aws.amazon.com/ja_jp/service-authorization/latest/reference/reference_policies_actions-resources-contextkeys.html)| -| IAM ポリシーに記載する Action, Resource, Condition の要素の中に、各サービスごとで具体的に何を記載できるか一覧になっているドキュメント。IAM ポリシーの Action 名とサービスごとの API 名が異なることがあるが、このドキュメントで Action 名から API 名も辿れる。|
|`200`| [ポリシーの評価論理 - AWS Identity and Access Management](https://docs.aws.amazon.com/ja_jp/IAM/latest/UserGuide/reference_policies_evaluation-logic.html)| -| AWS のサービスがリクエストを受け取って許可か拒否を決定するためのフローチャートが載っているドキュメント。|
|`200`| [IAM と連携する AWS サービス - AWS Identity and Access Management](https://docs.aws.amazon.com/ja_jp/IAM/latest/UserGuide/reference_aws-services-that-work-with-iam.html)| -| IAM ポリシーを利用してアクセス制御をする際に、各サービスごとの「`Resource` 要素に ARN 指定」「リソースベースのポリシー」「リソースタグ」「サービスにリンクされたロール」がサポートされているか一覧になっているドキュメント。[このアクション、ABAC ないし RBAC に対応してる？難解な IAM リファレンスに立ち向かうための地図を描いてみた - DevelopersIO](https://dev.classmethod.jp/articles/iam-reference-map-abac-rbac/) や [このアクション、タグベースの認可 ないし リソースレベルのアクセス許可 に対応してる？ IAM ポリシービジュアルエディタでお手軽に確認しちゃおう - DevelopersIO](https://dev.classmethod.jp/articles/iam-visual-editor-reference/) も参考になる。|
|`200`| [【実録】アクセスキー流出、攻撃者のとった行動とその対策 - DevelopersIO](https://dev.classmethod.jp/articles/accesskey-leak/)| -| アクセスキーを利用してどのように不正な操作がされたかの経験談とその対策。[[AWS利用者必読] アクセスキー漏洩による不正利用について - DevelopersIO](https://dev.classmethod.jp/articles/unauthorized-use-of-aws-access-keys-due-to-leakage/) にもアクセスキー利用の注意点について記載されているのでこちらも参考に。|
|`300`| [アクセス許可の境界を使用して IAM ユーザーとロールの範囲を限定し、権限の昇格を防ぐにはどうすればよいですか? - AWS ナレッジセンター](https://aws.amazon.com/jp/premiumsupport/knowledge-center/iam-permission-boundaries/)| -| アクセス許可の境界(Permission Boundary)のポリシー例。Permission Boundary によって課題を解決した実例は [AWS IAMの属人的な管理からの脱却【DeNA TechCon 2021】/techcon2021-19 - Speaker Deck](https://speakerdeck.com/dena_tech/techcon2021-19) が参考になる。|
|`300`| [PrincipalTag、ResourceTag、RequestTag、および TagKeys 条件キーを使用して、タグベースの制限のための IAM ポリシーを作成するにはどうすればよいですか? - AWS ナレッジセンター](https://aws.amazon.com/jp/premiumsupport/knowledge-center/iam-tag-based-restriction-policies/)| -| PrincipalTag、ResourceTag、RequestTag、および TagKeys の各条件キーを使用したサンプルの IAM ポリシーが記載されている。[AWSのABAC(タグに基づいたアクセス制御)の設計/運用のポイントを考える - DevelopersIO](https://dev.classmethod.jp/articles/aws-abac-tips/) も併せて読むとわかりやすい。|
|`300`| [Principal 要素で IAM ロールを指定するのと IAM ロールを引き受けたセッションを指定するのは何が違うのか？ 72 個のパターンで考えてみた - DevelopersIO](https://dev.classmethod.jp/articles/principal-element-iam-role-or-role-session/)| -| リソースベースポリシーの Principal 要素で `{ "AWS": "arn:aws:iam::AWS-account-ID:role/role-name" }` と `{ "AWS": "arn:aws:sts::AWS-account-ID:assumed-role/role-name/role-session-name" }` を指定した場合の違いがまとめられている。|

## Kinesis
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [DevDay 2019 - KinesisとLambdaでつくる Serverlessなログ基盤](https://pages.awscloud.com/rs/112-TZM-766/images/C-2.pdf)| -| Kinesis Data Streams を利用して EC2 や ECS からログを送信するパターンがいくつかわかりやすい構成図と共に記載されている。|

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

## Network Firewall
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [AWS Network Firewall 応⽤編1 - 新機能 MSRの活⽤/トラフィックを集約して監査する](https://d1.awsstatic.com/webinars/jp/pdf/services/202110_AWS_Black_Belt_Network_Firewall_advanced01.pdf)| -| [2021/08/30 に VPC ルートテーブルの新機能](https://aws.amazon.com/jp/blogs/news/inspect-subnet-to-subnet-traffic-with-amazon-vpc-more-specific-routing/)で、デフォルトのローカルルート（VPC 全体の CIDR 範囲）よりも小さな CIDR 範囲を指定してターゲットを詳細に指定できるようになった。これ以降、Network Firewall のサブネット設計の選択肢が増えてインターネット GW の内側の最初に Network Firewall エンドポイントのサブネットを配置しなくて良くなった。2021/08/30 以前に作成されたドキュメントの Network Firewall のサブネット設計を見る場合は注意。こちらの資料に書かれている構成から検討した方が良い。|
|`200`| [[アップデート] AWS Network Firewall でAWSが提供するマネージドのSuricata互換のIPSルール「AWS Managed Threat Signatures」が使えるようになりました - DevelopersIO](https://dev.classmethod.jp/articles/aws-network-firewall-threat-signatures/)| -| マルウェア、ボットネット、ウェブ攻撃、新興イベントなど、脅威を防御する侵入検知と防止のシグネチャーに、ステートフルのマネージドルールを活用できる。SNS を通じて、マネージドルールグループ更新の通知も可能。|
|`300`| [AWS Network Firewallのデプロイモデル - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/networking-and-content-delivery-deployment-models-for-aws-network-firewall/)| -| 分散型：個々のVPCにデプロイするモデル、集約型：East-West（VPCからVPC）やNorth-South（インターネットやオンプレミスへの通信）のトラフィックを集約する検査用VPCにデプロイするモデル、複合型：分散型と集約型の組み合わせごとのサブネットとルートテーブルの設計図が図でまとめられている。|

## Organizations
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [AWS Organizations で使用できる AWS のサービス - AWS Organizations](https://docs.aws.amazon.com/ja_jp/organizations/latest/userguide/orgs_integrate_services_list.html)| -| Organizations で使用できるサービスごとに、信頼されたアクセス/別アカウントを委任管理者にする機能がサポートされているかどうかの一覧。|
|`200`| [Organizing Your AWS Environment Using Multiple Accounts - Organizing Your AWS Environment Using Multiple Accounts](https://docs.aws.amazon.com/whitepapers/latest/organizing-your-aws-environment/organizing-your-aws-environment.html)| -| Organizations の OU の分け方などの推奨方法などがまとめられているホワイトペーパー。|
|`200`| [[AWS Organizations] SCP(サービスコントロールポリシー)の継承の仕組みを学ぼう - DevelopersIO](https://dev.classmethod.jp/articles/organizations-scp-inheritance/)| -| SCP の継承の考え方や、暗黙の Deny の概念が図でわかりやすい。|

## Outposts
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [【日本初導入】 AWS Outposts ラックを徹底解説 第1回 〜導入・利用方法の概要〜 - NTT Communications Engineers' Blog](https://engineers.ntt.com/entry/2022/03/15/102459)| -| AWS Outposts ラックの仕様、導入方法、利用方法について、Outposts ならではの注意点なども踏まえて記載されている。|

## RDS
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [Amazon RDS アーキテクチャ概要](https://pages.awscloud.com/rs/112-TZM-766/images/01_RDS_Architecture.pdf)| -| [2020/10/15に開催された第2回 Amazon RDS Online Seminar](https://aws.amazon.com/jp/blogs/news/amazon-rds-online-seminar2-qa-202011/)の資料。|
|`200`| [Amazon Aurora アーキテクチャ概要](https://pages.awscloud.com/rs/112-TZM-766/images/01_Amazon%20Aurora%20%E3%82%A2%E3%83%BC%E3%82%AD%E3%83%86%E3%82%AF%E3%83%81%E3%83%A3%E6%A6%82%E8%A6%81.pdf)| -| [2020/09/10に開催された第1回 Amazon RDS Online Seminar](https://aws.amazon.com/jp/blogs/news/amazon-rds-online-seminar1-qa-202009/)の資料。[Aurora が⾼いパフォーマンスを発揮する理由](https://pages.awscloud.com/rs/112-TZM-766/images/01_Amazon%20Aurora%20%E3%82%A2%E3%83%BC%E3%82%AD%E3%83%86%E3%82%AF%E3%83%81%E3%83%A3%E6%A6%82%E8%A6%81.pdf#page=31)も。|
|`200`| [Amazon RDS Online Seminar 「忘れちゃいけない！Amazon RDS/Amazon Aurora のアップグレードとその方法」資料・動画及び QA 公開 - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/amazon-rds-online-seminar-20210617/)| -| 2021/6/17に開催した Amazon RDS Online Seminar「忘れちゃいけない！Amazon RDS/Amazon Aurora のアップグレードとその方法」の資料・動画。|
|`200`| [新しい Amazon RDS のマルチ AZ 配置オプション – MySQL および PostgreSQL データベースでご利用可能 - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/amazon-rds-multi-az-db-cluster/)| -| マルチ AZ DB クラスターの特徴（インスタンスが提供するローカルストレージを使用してトランザクションログを保存/フェイルオーバーにかかる時間/ホットスタンバイ/レプリケートはトランザクションログのみでクォーラムメカニズムを使用）などがまとめられている。|
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
|`200`| [Amazon S3 セキュリティベストプラクティスの実践（権限管理のポリシー) – 前編 - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/introducing-s3-security-best-practices-1/)| -| アイデンティティベースのポリシー、リソースベースのポリシー、VPC エンドポイントポリシー、サービスコントロールポリシーをそれぞれ異なる目的のために使い分ける方法など。[後編](https://aws.amazon.com/jp/blogs/news/introducing-s3-security-best-practices-2/) もある。|
|`300`| [S3のコストを大幅に削減した話 - Gunosy Tech Blog](https://tech.gunosy.io/entry/s3_costcut)| -| gzip の特徴を活かして、複数の gzip ファイルを MultipartUpload で 単一の gzip ファイルにすることで、ストレージクラス変更時の Glacier への PUT リクエストの回数を減らし、コスト削減させた。|
|`400`| [Diving Deep on S3 Consistency (English)](https://www.allthingsdistributed.com/2021/04/s3-strong-consistency.html)| -| S3で整合性を保つための仕組みを解説。|
|`---`| [AWS 導入事例：株式会社テレビ東京](https://aws.amazon.com/jp/solutions/case-studies/tv-tokyo/)| -| 13PB のテレビ映像アーカイブを Amazon S3 / S3 Glacier へ移行。|

## Security Hub
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [新学期セキュリティスタートダッシュ Security Hub 編](https://pages.awscloud.com/rs/112-TZM-766/images/20220428_17th_ISV_DiveDeepSeminar_Security_Hub.pdf)| [`Vidyard`](https://play.vidyard.com/JhTTR1GGHgstRkAg5ENhd2)| [【開催報告】アップデート紹介とちょっぴり DiveDeep する AWS の時間 第十七回 (04/28) - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/update-divedeep-series-17/) のセッション。Security Hub を導入するために知りたい内容を基本的な2022年4月時点の最新情報込みで。|

## SCT
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| 第十九回 ちょっぴりDD - イチから覚える AWS Schema Conversion Tool | [`YouTube`](https://www.youtube.com/watch?v=JHrqArrH3AE)| SCT の基本的な使い方を動画で解説。|

## Shield
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [AWS Shield Advanced のアップデート – アプリケーションレイヤー DDoS の自動緩和 - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/aws-shield-advanced-update-automatic-application-layer-ddos-mitigation/)| -| 従来は Shield Advanced を利用することでベースラインからの著しい逸脱したリクエストは DDoS イベントとしてフラグが設定され、Amazon CloudWatch を通じてアラートがトリガーされるので、悪意のあるトラフィックを分離する AWS WAF ルールを手動で作成し、AWS WAF コンソールまたは API を介してデプロイし、ルールの有効性を評価する必要があった。このプロセスには DDoS 攻撃を緩和するまでに時間がかかってしまっていたが、AWS WAF ルールが自動的に作成、テスト、デプロイされ、お客様に代わってレイヤー 7 の DDoS イベントを緩和する機能が提供されたので、利用手順がまとめられている。|

## Site-to-Site VPN (サイト間 VPN)
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`300`| [[AWS] Site to Site VPN の BGP 経路を制御しよう - DevelopersIO](https://dev.classmethod.jp/articles/control-bgp-route-on-site-to-site-vpn/)| -| Site-to-Site VPN を利用した場合の2つのトンネルと Virtual Private Gateway(VGW), Transit Gateway を利用した場合の BGP による経路制御の方法が分かりやすくまとめっている。|
|`300`| [Simulating Site-to-Site VPN Customer Gateways Using strongSwan - AWSNetworking & Content Delivery](https://aws.amazon.com/blogs/networking-and-content-delivery/simulating-site-to-site-vpn-customer-gateways-strongswan/)| -| AWS 環境のみで擬似的にオンプレミスのネットワークを作成し、Site-toSite VPN を構築する手順。Certificate-based な [part 2](https://aws.amazon.com/blogs/networking-and-content-delivery/simulating-site-to-site-vpn-customer-gateways-using-strongswan-part-2-certificate-based-authentication/)もある。|

## Snowball
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [AWS Snowball Edge を使ってみた！ 全工程レポート - ⬢ Appirits spirits](https://spirits.appirits.com/type/technology/14856/)| -| 注文から返送までの流れ、機材の詳細なレポートなど。|
|`---`| [AWS 導入事例：KDDI株式会社 - AWS](https://aws.amazon.com/jp/solutions/case-studies/kddi_2022/)| -| 252台の AWS Snowball Edge を活用して25PBの大容量データ移行を約2年で完遂した事例。|

## Snowmobile
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`---`| AWS re:Invent 2016: Move Exabyte-Scale Data Sets with AWS Snowmobile| [`YouTube`](https://youtu.be/8vQmTZTq7nw)| AWS re:Invent 2016 での Snowmobile 発表の動画。[ここの59秒あたり](https://youtu.be/8vQmTZTq7nw?t=59)から実物が登場する衝撃だけはほぼ忘れられない瞬間。|

## Systems Manager
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [AWS Systems Manager(SSM) の数多い機能群を攻略するための図を書いてみた 2021 - DevelopersIO](https://dev.classmethod.jp/articles/all-ssm-capabilities-2021/)| -| Systems Manager の機能一覧が把握しやすい図。|
|`200`| [情シス向け運用ユースケース - AWS Summit 2021](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-51_AWS_Summit_Online_2021_ManagementOnAws.pdf)| [`YouTube`](https://youtu.be/c5MFQLggfQ0)| Systems Manager を利用したサーバーのインベントリ可視化、パッチ適用、リモートアクセス、一括管理などのユースケースがまとめられている。|
|`200`| [AWSでSSMエージェントの自動更新をCloudFormationのスタックセット(StackSets)で複数のリージョンやアカウントに適用](https://zenn.dev/sugikeitter/articles/automating-updates-to-ssm-agent-with-cfn-stacksets)| -| マルチアカウント環境などで全てのサーバーのSSMエージェントの自動更新させる方法。|
|`200`| [CloudFormation で cfn-init に代えて State Manager を利用する方法とその利点 - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/using-state-manager-over-cfn-init-in-cloudformation-and-its-benefits/)| -| CloudFormation で EC2 インスタンスをデプロイした後に、ソフトウェアのインストール、またはオペレーティングシステムの設定をする方法。|
|`300`| [AWS IAMの安全な管理方法 · DeNA Engineers' Blog](https://engineer.dena.com/posts/2019.12/aws-iam-management/)| -| IAM ロールが利用できないシステムからAWSサービスへのアクセス時に、定期的にIAMユーザのシークレットアクセスキーのローテートを行う方法。|

## SQS
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| SQS 標準キューのCLIを利用した動作デモ| [`YouTube`](https://www.youtube.com/watch?v=8cAk1_GSV0g&t=336s)| 動画なのでプロデューサー・キュー・コンシューマーの関係がわかりやすい。順序保証がないことや、コンシューマーを増やすことで処理量が線形的に増えていくことがわかる。|
|`200`| SQS FIFOキューのCLIを利用した動作デモ| [`YouTube`](https://www.youtube.com/watch?v=8cAk1_GSV0g&t=660s)| 標準キューと比較してコンシューマーが増えても処理量が線形的に増えるわけではないことや、並列化をしたい場合のグループID利用、プロデューサーからの重複排除が可能なことがわかる。|
|`300`| [マルチテナントソリューションでAmazon SQSを使う - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/using-amazon-sqs-in-a-multi-tenant-saas-solution/)| -| SaaS ソリューションを構築する際の一般的なシナリオを紹介し、データ分離、スケーラビリティ、コンプライアンス要件が、キューイングモデルの選択にどのように関係するかを説明。|
|`---`| [クックパッドの機械学習を支える基盤のつくりかた - AWS Summit Tokyo 2017](https://d1.awsstatic.com/events/jp/2017/summit/slide/D3T5-2.pdf)| -| 時間のかかる料理画像の自動認識処理を SQS を利用することで非同期なアーキテクチャとして実現。|
|`---`| [Sansanがメッセージング (SQS) でスケーラビリティを手に入れた話](https://www.slideshare.net/atsushikambara/sansan-sqs)| -| SQS で非同期な設計にすることでデータベースの負荷の増減を安定させたり、システム全体は止まらせないままで部分的にメンテナンスを行ったりなど。|
|`---`| [1日300万件のレコードを処理するアーキテクチャ構成　保育士さんの負担はDesign for Failureな「午睡チェック」でサポート - ログミーTech](https://logmi.jp/tech/articles/325091)| -| DynamoDB への書き込みの間に SQS を挟むことで書き込み量にスパイクが発生しないよう平準化させている。|

## SSO
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [Azure AD と AWS SSOの連携 - fu3ak1's tech days](https://fu3ak1.hatenablog.com/entry/2020/12/20/000622)| -| IdP として Azure Active Directory を利用したAWS SSO の構築方法。|
|`200`| [AWS クラウドサービス活用資料集 - AWSアカウント シングルサインオンの設計と運用 #IDフェデレーションで変わる運⽤の論点](https://d1.awsstatic.com/webinars/jp/pdf/services/20200722_AWSBlackbelt_%E3%82%B7%E3%83%B3%E3%82%B0%E3%83%AB%E3%82%B5%E3%82%A4%E3%83%B3%E3%82%AA%E3%83%B3%E3%81%AE%E8%A8%AD%E8%A8%88%E3%81%A8%E9%81%8B%E7%94%A8.pdf#page=53)| -| 権限セット数に制限がある中で多くのアカウントを管理する場合、 RBAC ではなく ABAC モデルの考え方について。|
|`200`| [AWS SSO、AD、ABACを触ってみる - サーバーワークスエンジニアブログ](https://blog.serverworks.co.jp/2021/04/16/113023)| -| ABAC の設定手順の一例が記載されている。|
|`---`| [AWS SSOでセキュアな管理とコスト削減　不正アクセス・サービス停止乗り越えたマルチアカウント対策 - ログミーTech](https://logmi.jp/tech/articles/324310)| -| AzureAD と AWS SSO 利用への移行理由と移行時のトラブルについても言及されている。|

## StepFunctions
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`300`| [AWS EXpert Online for JAWS-UG 18 - 見せてやるよ、Step Functions の本気ってやつをな](https://www.slideshare.net/AmazonWebServicesJapan/aws-expert-online-for-jawsug-18-step-functions) | [`YouTube`](https://www.youtube.com/watch?v=DcE_c8_6QUk) | 一連のワークフローのリポジトリ分けの観点やデバッグについての考え方、Step Functions を動かして終わりの状態からより実践的な利用方法について学べる。|
|`300`| [分散システムにおけるSagaパターンのAWS Step Functions による実装 #AWSDevDay - Speaker Deck](https://speakerdeck.com/fatsushi/fen-san-sisutemuniokerusagapatanfalseaws-step-functions-niyorushi-zhuang-number-awsdevday)| -| Saga パターンについての話と、Step Functions によるエラーハンドリングとリトライ、[e-コマースの注文処理のサンプル実装例](https://github.com/aws-samples/aws-step-functions-long-lived-transactions)など。|

## Transit Gateway
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [クロスアカウントな AWS Transit Gateway を、絵で見て（完全に）理解する。 - DevelopersIO](https://dev.classmethod.jp/articles/transitgateway-cross-account-diagram/)| -| Transit Gateway コンポーネントの位置関係、関連付け（アソシエーション）と伝播（プロパゲーション）が絵でわかりやすい。|
|`200`| [Field Notes: Working with Route Tables in AWS Transit Gateway - AWS Architecture Blog](https://aws.amazon.com/blogs/architecture/field-notes-working-with-route-tables-in-aws-transit-gateway/)| -| 複数の VPC とルートテーブルの関係の一枚絵がわかりやすい。|
|`---`| [グノシーにおける AWS Transit Gateway 活用事例 - Gunosy Tech Blog](https://tech.gunosy.io/entry/gunosy-aws-transit-gateway)| -| 複数のアカウントと VPC に Direct Connect を接続していたが、 Transit Gateway で設計がシンプルになって考慮する点やリードタイムが減った話。|
|`---`| [AWS 導入事例：株式会社マネーフォワード - AWS](https://aws.amazon.com/jp/solutions/case-studies/moneyforward/)| -| マルチアカウント構成で Transit Gateway を活用しながら EKS クラスタと他のアカウントのリソースへ接続している。|
|`---`| [AWS導入事例: SMK株式会社 AWS Transit Gateway Inter-Region Peeringを活用したグローバルネットワークHub](https://aws.amazon.com/jp/blogs/news/smk-corporation-aws-transit-gateway-inter-region-peering/)| -| AWS Transit Gateway Inter-Region Peering を活用し、AWSの閉域ネットワークを国内から海外拠点まで適用することで、構築時間やコストを削減。|

## Trusted Advisor
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [AWS Trusted Advisor のベストプラクティスチェックリスト - AWS](https://aws.amazon.com/jp/premiumsupport/technology/trusted-advisor/best-practice-checklist/)| -| コストの最適化、セキュリティ、耐障害性、パフォーマンス、サービスの制限といった AWS のベストプラクティスに基づく 5 つのカテゴリにわたるチェックと推奨事項。|

## VPC endpoints (VPCe) / PrivateLink
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [2つのVPCエンドポイントの違いを知る - DevelopersIO](https://dev.classmethod.jp/articles/vpc-endpoint-gateway-type/)| -| ゲートウェイ型とインターフェイス型の2種類の経路違いが図で簡潔にまとめられている。|
|`300`| [「Amazon S3 インターフェースエンドポイント（PrivateLink）ではプライベート DNS をサポートしていません」 の意味を絵をかいて腹落ちさせてみた - DevelopersIO](https://dev.classmethod.jp/articles/s3-privatelink-diagram/)| -| PrivateLink を利用した場合に設定される DNS 名が整理されている。|
|`---`| [住信SBIネット銀行の PrivateLink 事例](https://pages.awscloud.com/rs/112-TZM-766/images/K1-02.pdf#page=27)| -| 提携企業へ利用してもらうシステムをインターネットに公開することなく PrivateLink を利用することで AWS のネットワークに閉じた形で複数企業へ提供している事例。|

## WAF
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [AWS WAFのAWS マネージドルールの動作をカスタマイズする方法 - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/how-to-customize-behavior-of-aws-managed-rules-for-aws-waf/)| -| マネージドルールグループの自動更新の制御（バージョン管理）方法や、カスタマイズする方法など。|
|`---`| [AWS WAF セキュリティオートメーション - AWS ソリューション](https://aws.amazon.com/jp/solutions/implementations/aws-waf-security-automations/)| -| 一般的なウェブベースの攻撃をフィルタリングするための、一連の AWS WAF (ウェブアプリケーションファイアウォール) ルールが自動的にデプロイされる仕組みの参照実装と手順。|
|`---`| [Log4jで話題になったWAFの回避/難読化とは何か - WAF Tech Blog - クラウド型 WAFサービス Scutum 【スキュータム】](https://www.scutum.jp/information/waf_tech_blog/2021/12/waf-blog-081.html)| -| AWS 関係なく WAF の実装の観点から防げるものが理解しやすく記載されている。|

# カテゴリ別

## Availability (可用性) / Multi Region (マルチリージョン)
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [Disaster recovery options in the cloud - Disaster Recovery of Workloads on AWS: Recovery in the Cloud](https://docs.aws.amazon.com/ja_jp/whitepapers/latest/disaster-recovery-workloads-on-aws/disaster-recovery-options-in-the-cloud.html)| -| 災害対策のホワイトペーパー。戦略の4パターン(バックアップとリストア/パイロットライト/ウォームスタンバイ/マルチアクティブ)と、AWS サービスを利用した具体的な設計事例など。このホワイトペーパーは AWS ブログで「ディザスタリカバリ (DR) アーキテクチャ」シリーズとして<br>・[パート I：クラウドでのリカバリの戦略](https://aws.amazon.com/jp/blogs/news/disaster-recovery-dr-architecture-on-aws-part-1-strategies-for-recovery-in-the-cloud/)<br>・[パート II: 迅速なリカバリによるバックアップと復元](https://aws.amazon.com/jp/blogs/news/disaster-recovery-dr-architecture-on-aws-part-ii-backup-and-restore-with-rapid-recovery/)<br>・[パート III: パイロットライトとウォームスタンバイ](https://aws.amazon.com/jp/blogs/news/disaster-recovery-dr-architecture-on-aws-part-iii-pilot-light-and-warm-standby/)<br>・[パート IV: マルチサイトアクティブ/アクティブ](https://aws.amazon.com/jp/blogs/news/disaster-recovery-dr-architecture-on-aws-part-iv-multi-site-active-active/)<br>でも解説されている。|
|`200`| [なぜ「AWS で負荷分散は３AZ にまたがるのがベストプラクティス」と言われるのか 可用性の面から考えてみた](https://dev.classmethod.jp/articles/202008-three-az-load-balancing/)| -| AZ が多い場合のメリットや過去の AZ 障害などの話。|
|`200`| [マルチリージョン、ちょっとその前に...-サービスの可用性について考える - AWS Summit Online 2021](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-53_AWS_Summit_Online_2021_Thinking-about-Availability.pdf) | [`Youtube`](https://www.youtube.com/watch?v=8MyZ84WEjrc)| マルチリージョン構成でのデータ整合性や切替⽅式などの重要な検討事項、ビジネスニーズとコストのバランスについて。|
|`200`| [Network視点で考えるシームレスなマルチリージョンへの移行と検討](https://pages.awscloud.com/rs/112-TZM-766/images/ORL-T3-Session.pdf)| -| マルチリージョン構成で Route53, Global Accelerator の違いなど。|
|`300`| [データベースの視点で考えるマルチリージョンアーキテクチャ](https://pages.awscloud.com/rs/112-TZM-766/images/ORL-T4-Session.pdf)| -| RDS, Aurora のマルチリージョン利用が簡潔にまとまっている。|

## Cache
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [Webアプリケーションのキャッシュ戦略とそのパターン / Pattern and Strategy of Web Application Caching - Speaker Deck](https://speakerdeck.com/moznion/pattern-and-strategy-of-web-application-caching)| -| キャッシュのメリット・デメリットとデザインパターン。|

## CI / CD
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [Amazonの事例に学ぶ継続的デリバリーによるリリース作業の改善 - AWS Innovate 2020](https://d1.awsstatic.com/events/jp/2020/innovate/pdf/S-20_AWSInnovate_Online_Conference_2020_Spring_CICD.pdf)| -| CI/CD やパイプラインの必要性と Amazon が過去にパイプラインを取り入れた時の効果など。|
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
|`200`| 【AWS Black Belt Online Seminar】 CON231 コンテナセキュリティ入門| `Youtube`|[Part.1 - 安全なイメージを作るための Dockerfile の書き方やイメージのスキャンについて](https://www.youtube.com/watch?v=I1o01lkQNHY) <br> [Part.2 - イメージをレジストリに保存してホストに届けるまで](https://www.youtube.com/watch?v=OTwC6zpgZjc) <br> [Part.3 - コンテナを起動させるホストについて](https://www.youtube.com/watch?v=drWE7enGFvo) <br> の三部作。|
|`300`| [コンテナランタイムの仕組みと、Firecracker、gVisor、Unikernelが注目されている理由。 Container Runtime Meetup #2 － Publickey](https://www.publickey1.jp/blog/20/firecrackergvisorunikernel_container_runtime_meetup_2.html)| -| CRI, OCI とは何か？コンテナランタイムの高レベルと低レベルについてなど。|

## Cost (料金)
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [AWSのコスト最適化/リザーブドインスタンス - AWS サービス別資料](https://d1.awsstatic.com/webinars/jp/pdf/services/20171110_AWS-BlackBelt_RI_update.pdf)| -| [損益分岐点についての図](https://d1.awsstatic.com/webinars/jp/pdf/services/20171110_AWS-BlackBelt_RI_update.pdf#page=71)が利用検討の参考になる。|

## Database (DB)
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [AWS が提供するクラウドデータベース - AWS](https://aws.amazon.com/jp/products/databases/)| -| AWS のデータベースサービス一覧やそれぞれの特徴、マネージドなデータベースを利用するメリットなど。|
|`100`| [NoSQL とは?（NoSQL データベースの解説と SQL との比較）- AWS](https://aws.amazon.com/jp/nosql/)| -| NoSQL (非リレーショナル) データベースの仕組みや、必要となる場面、NoSQL データベースのタイプなどがまとめられている。|
|`100`| [AWS のデータベースサービスはなぜ複数存在するのか - builders.flash☆ - 変化を求めるデベロッパーを応援するウェブマガジン - AWS](https://aws.amazon.com/jp/builders-flash/202207/reason-plural-databases/)| -| RDB が分散処理と相性が悪いため、可用性や性能を重視して整合性は結果的に取れていれば良い BASE という別の考え方で用途によっては NoSQL のプロダクトが拡大した背景の説明。列指向データベース、キーバリューストア、時系列データベース、台帳データベース、グラフ指向データベース、ドキュメント型データベースなどについても簡易的な言及がある。|
|`100`| [社内SQL研修のために作った資料を公開します - 株式会社AI Shift](https://www.ai-shift.co.jp/techblog/1980)| -| SQL や RDB とは？が簡潔にまとめられている。|
|`100`| [NoSQL とは?（NoSQL データベースの解説と SQL との比較）- AWS](https://aws.amazon.com/jp/nosql/)| -| NoSQL についてのわかりやすい解説、 RDB との使い分けの参考になるような一般的な特徴の比較がまとめられている。|

## Data Lake (データレイク) / Data Warehouse (DWH・データウェアハウス)
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [レイクハウスアーキテクチャとは - Amazon Web Services](https://aws.amazon.com/jp/big-data/datalakes-and-analytics/data-lake-house/)| -| レイクハウスアプローチの仕組みや必要になる理由についてなど。|
|`200`| [貯めるだけじゃもったいない！AWS 分析サービスを使ったデータレイクの有効活用 - AWS Summit Online 2021](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-06_AWS_Summit_Online_2021_ANT01.pdf) | [`YouTube`](https://www.youtube.com/watch?v=95P_6_CJeys)| データレイクについての説明や、AWS でデータレイクを活用するときのサービスの紹介。|
|`300`| [「ふくおかＦＧ ＤＸ推進基盤の構築」～おいしいデータレイクの作り方～ - AWS Summit 2020](https://pages.awscloud.com/rs/112-TZM-766/images/CUS-54_AWS_Summit_Online_2020_FFG.pdf)| -| データ分析の必要性から、 Glue と AWS サービスを組み合わせて分析の仕組みをどのように構築したかが段階的に説明されている。|

## Developing
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [The Twelve-Factor App （日本語訳）](https://12factor.net/ja/)| -| 多種多様なSaaSアプリケーション開発現場での経験と観察をまとめた、ソフトウェア開発の方法論。|
|`200`| [「The Twelve-Factor App」を15項目に見直した「Beyond the Twelve-Factor App」を読んだ - kakakakakku blog](https://kakakakakku.hatenablog.com/entry/2020/03/09/084833)| -| クラウド化が進み技術的な変化も踏まえて「Beyond the Twelve-Factor App」がアップデートされた内容を簡潔にまとめたもの。|
|`200`| [サイバーエージェントのフィーチャーフラグを活用した高速開発【CADC2022】 - Speaker Deck](https://speakerdeck.com/cyberagentdevelopers/saibaezientofalsehuitiyahuraguwohuo-yong-sitagao-su-kai-fa-cadc2022)| -| フィーチャーフラグとは何か、メリットデメリットが簡潔にまとめられている。|
|`300`| [Boto3(AWS SDK for Python)をコードリーディングして仕組みを理解する](https://zenn.dev/sugikeitter/articles/6648845968cec6)| -| Boto3 のクライアント API とリソース API の実装の違い、boto3 の役割と botocore の役割の違いなど。|

## DevOps
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [DevOpsとは何か？ そのツールと組織文化、アジャイルとの違い - Build Insider](https://www.buildinsider.net/enterprise/devops/01)| -| DevOps の概念の原典や目的、"開発チーム（Development）と運用チーム（Operations）がお互いに協調し合うことで、開発・運用するソフトウェア／システムによってビジネスの価値をより高めるだけでなく、そのビジネスの価値をより確実かつ迅速にエンドユーザーに届け続ける"や、開発チームと運用チームの役割の違いによる対立構造がまとまっている。|
|`100`| [デロイト トーマツ ウェブサービス株式会社(MMM)は『AWS DevOps コンピテンシー』認定を取得しました - デロイト トーマツ ウェブサービス株式会社（DWS）公式ブログ](https://blog.mmmcorp.co.jp/blog/2020/09/24/aws_competency_program_devops/)| -| 記事の中にある [DevOps の構成要素を表す図](https://blog.mmmcorp.co.jp/images/aws_competency_program_devops/devops.png) がわかりやすい。|
|`100`| [DevOpsトポロジー - Ryuzee.com](https://www.ryuzee.com/contents/blog/14567)| -| DevOps トポロジーのアンチタイプとそうでないもののパターンと解説が簡潔にまとめられている。|
|`100`| [「コード書きました、あとはよろしく」では優れたソフトウェアは生まれない　コンテナのスペシャリストが語る、運用性を損なう8つの実装例 - ログミーTech](https://logmi.jp/tech/articles/325995)| -| Amazon AWS の CTO である Werner Vogels の「You build it, you run it」という言葉を、この言葉が使われた前後の文章を含めて「開発と運用の両者が共通のゴールを持って、共同して、運用上の責任を持つことがとても大事だ」と解説している。|
|`100`| [マイクロサービスの失敗は技術だけの問題か――Amazonに学ぶ開発・運用組織の理想形とは (1/2)：CodeZine（コードジン）](https://codezine.jp/article/detail/15284)| -| マイクロサービスを採用しても、適切な権限委譲ができておらず、それぞれのチームが全ての工程に責任を持っている状態でなければうまくいかない場合もあるという話（p.2）など、マイクロサービス はあくまで手段であることが簡潔に語られている。|
|`200`| [Amazon S3を開発・運用する方法 - 巨大なマイクロサービスと組織 - AWS Summit Online 2020](https://pages.awscloud.com/rs/112-TZM-766/images/AWS-33_AWS_Summit_Online_2020_STG01.pdf)| [`AWS`](https://resources.awscloud.com/vidyard-all-players/aws-33-aws-summit-online-2020-720p-2)| S3 の開発チームの DevOps の手法や、そのための組織構成など。|
|`200`| [CIOpsとGitOpsの話 - inductor's blog](https://blog.inductor.me/entry/2021/09/24/015402)| -| 「CIOpsとGitOpsの一番の違いは、Push型かPull型か」であり、それぞれのメリットデメリットがまとめられている。|
|`300`| [DB変更リリースの停止時間を最小化するには？「DevOps with Database on AWS」 #AWSDevDay - DevelopersIO](https://dev.classmethod.jp/articles/devops-with-database/)| -| ライフサイクルが異なるアプリケーションとデータベースに対する変更を適切に管理することを目的として、代表的なデータベーススキーマ変更の手法を紹介し、それを CI/CD パイプラインに組み込む方法について検討している。|

## DevSecOps
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [DevSecOpsとは何か — 導入する組織が増加している理由 - メルカリエンジニアリング](https://engineering.mercari.com/blog/entry/20201214-bea4717e9a/)| -| DevSecOps の5つのコンセプトや注目されている理由など。|

## Infrastructure as Code (IaC)
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [Infrastructure as Code (IaC) 談義 2022 ~AWS Developer Live Show](https://www.slideshare.net/AmazonWebServicesJapan/infrastructure-as-code-iac-2022-251672484)| [`Youtube`](https://www.youtube.com/watch?v=ed35fEbpyIE)| IaC の必要性、課題、考慮すべき部分など。|
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
|`100`| [これなら分かる！ マイクロサービス（入門編）～モノリスと比較した特徴、利点と課題 (1/3)：CodeZine（コードジン）](https://codezine.jp/article/detail/11055)| -| マイクロサービスの特徴が簡潔にまとまっている。（ユーザー登録必要）|
|`100`| [ASCII.jp：なぜAmazonはマイクロサービスに舵を切ったのか？](https://ascii.jp/elem/000/001/620/1620756/)| -| Amazon.com のシステムがモノリシックアーキテクチャのアンチパターンにハマってしまい、ビジネスの急成長にシステムのスケールや機能追加が追いつかなり、マイクロサービスに大きく方向転換した背景について。また、すべてのチームが担当するサービスのすべての所有権、説明責任、より良くしようとする動機を持つべきという姿勢がすべてのエンジニアに浸透し、Amazon.com の機能はマイクロサービス化できたとのこと。最後に AWS の歴史の話もちょこっと記載されている。|
|`200`| [スタートアップのためのマイクロサービス入門 - AWS Startup ブログ](https://aws.amazon.com/jp/blogs/startup/techblog-microservices-introduction/)| -| マイクロサービスとは何か？必要かどうかについての考え方についてなど。`「マイクロサービス」という言葉の功罪` という章以降を一読するのがおすすめ。|

## Migration (マイグレーション・移行)
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [マイグレーションを実現するために - 第 1 回 : 既存システムのマイグレーションはなぜ必要なのか ? - builders.flash☆](https://aws.amazon.com/jp/builders-flash/202010/migration-to-cloud/?awsf.filter-name=*all)| -| クラウドへの移行の必要性や段取りがまとめられている。[第2回](https://aws.amazon.com/jp/builders-flash/202011/migration-to-cloud-2/?awsf.filter-name=*all)、[第3回](https://aws.amazon.com/jp/builders-flash/202102/migration-to-cloud-3/?awsf.filter-name=*all)のシリーズもの。|
|`200`| [Amazon RDS for Oracle / SQL Server への移行ベストプラクティス - AWS Summit 2019](https://pages.awscloud.com/rs/112-TZM-766/images/B3-01.pdf)| -| 考えられる移行パスや、ニアゼロダウンタイム移行の一例など。|
|`200`| [AWSのサービスを使ったオンプレミスからのデータベース移⾏ - AWS Summit Online 2020](https://pages.awscloud.com/rs/112-TZM-766/images/AWS-18_AWS_Summit_Online_2020_DAT01.pdf)| -| データベースを移⾏する際のパターン、SCT/DMSを活⽤したデータベース移⾏の具体例など。|

## Monitoring / Observability (モニタリング・監視 / オブザーバビリティ・可観測性)
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [モニタリングとオブザーバビリティ - AWS マネジメントとガバナンス](https://aws.amazon.com/jp/products/management-and-governance/use-cases/monitoring-and-observability/)| -| AWS のオブザーバビリティの定義。|
|`100`| [オブザーバビリティ（可観測性）入門ガイド - New Relic](https://newrelic.com/jp/resources/ebooks/the-age-of-observability)| -| New Relic の考え方だが、"監視とはエラーや問題の発生時に迅速に対応できるようにする、「データを収集」することを目的としてシステムを構築することです。一方、可観測性とはエラーや問題が発生したことを検知するだけでなく、それが「なぜ」起きたのか、その原因を探り、改善のアクションに繋げることを目的としてデータを収集します。"というのがわかりやすい。|
|`100`| [これからのSREはモニタリングからオブザーバビリティへ APMやEUMを使いこなせ【デブサミ2021】 (1/2)：CodeZine（コードジン）](https://codezine.jp/article/detail/13696)| -| 単なるモニタリング結果の報告か、モニタリング結果を元に調査できるかの具体例がわかりやすい。|
|`200`| [SIEM on Amazon OpenSearch Service](https://github.com/aws-samples/siem-on-amazon-opensearch-service/blob/main/README_ja.md)| -| [Security information and event management (SIEM)：セキュリティ情報とイベント管理](https://docs.aws.amazon.com/ja_jp/wellarchitected/latest/management-and-governance-lens/security-information-and-event-management-siem-1.html) を Amazon OpenSearch Service を利用して AWS サービスのログの可視化やセキュリティ分析を実現する仕組み。ワンクリックで Amazon OpenSearch Service とそれ用の S3 バケットが構築され、[あとは対象にしたいサービスごとにログを S3 バケットに保存する手順を実施](https://github.com/aws-samples/siem-on-amazon-opensearch-service/blob/main/docs/configure_aws_service_ja.md) すれば、各サービスのログごとのフォーマット作業をせずに[用意されたダッシュボード](https://github.com/aws-samples/siem-on-amazon-opensearch-service/blob/main/docs/dashboard_ja.md)を利用できる。|
|`200`| [AWS Startup Tech Meetup #3: かんたんコンテナロギング選手権](https://speakerdeck.com/prog893/aws-startup-tech-meetup-number-3-kantankontenaroginguxuan-shou-quan)| -| コンテナのログのよくある課題、ログの種類や転送方法、格納先、サンプルアーキテクチャ。|
|`300`| [KubernetesでFluentdの信頼性を担保するための3つの観点](https://zenn.dev/taisho6339/articles/eff38b47cbdbcb)| -| マイクロサービスやコンテナのログでよく利用される Fluentd の信頼性について。|

## Multi Account (マルチアカウント)
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [AWSアカウントはなぜ＆どう分けるべき？ - NRIネットコムBlog](https://tech.nri-net.com/entry/why_multi_accounts)| -| 前半でシングルアカウントの課題が綺麗にまとまっている。|
|`200`| [これが基本のマルチアカウント管理 - AWS Expert Online for JAWS-UG #15](https://www.slideshare.net/AmazonWebServicesJapan/20210526-aws-expert-online) | [`YouTube`](https://www.youtube.com/watch?v=3QJ-RA5R0Jk)| マルチアカウント管理の必要性や考え方、ベストプラクティス、Control Tower による LandingZone の実現、具体的なガードレールの実装。アカウント分割により管理できる例が[ここ](https://www.slideshare.net/AmazonWebServicesJapan/20210526-aws-expert-online/7)や[Landing Zone とは](https://www.slideshare.net/AmazonWebServicesJapan/20210526-aws-expert-online/26)の説明がわかりやすい。|
|`200`| [「AWS Control Towerを利用したマルチアカウント管理とセキュリティ統制」JAWS DAYS 2021登壇資料 #jawsug #jawsdays #jawsdays2021 #jawsdays2021_C - DevelopersIO](https://dev.classmethod.jp/articles/jaws-days-2021-control-tower/)| [`YouTube`](https://youtu.be/JpJjJ39c5oQ)| [ここ](https://speakerdeck.com/cmusudakeisuke/aws-control-towerwoli-yong-sitamarutiakauntoguan-li-tosekiyuriteitong-zhi?slide=10)からのアカウントを分けることによる分離の考え方の図がわかりやすい。|
|`200`| [AWS Organizationsを活用したマルチアカウントのセキュリティサービス使用方法 ～まとめ～ - fu3ak1's tech days](https://fu3ak1.hatenablog.com/entry/2021/01/28/002536)| -| Organizationsを活用したセキュリティサービスについての紹介。|
|`200`| [JAWS-UG 情シス / AWS Sandbox環境の運用と管理 - Speaker Deck](https://speakerdeck.com/sumi/aws-sandboxhuan-jing-falseyun-yong-toguan-li)| -| 検証環境のため、定期的にリソース削除する仕組みを Organizations のアカウント解約機能を使いつつ、自由度+コストの問題に対応してる話|
|`300`| [AWS Organizations における組織単位のベストプラクティス - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/best-practices-for-organizational-units-with-aws-organizations/)| -| AWS が推奨する「ランディングゾーン」と呼ばれる安全かつ生産性の高いマルチアカウント AWS 環境を構築する要素について。組織単位 (Organization Unit: OU) の分割方法など。|
|`---`| [【オンラインMeetup イベントレポート】第一回 AWSマルチアカウント事例祭り - ZOZO TECH BLOG](https://techblog.zozo.com/entry/20200908-meetup-report) / [`logmi 書き起こし`](https://logmi.jp/events/2464)| [`YouTube`](https://www.youtube.com/watch?v=OV7r1xWuvSg)| 1. AWS Configを用いたマルチアカウント・マルチリージョンでのリソース把握とコンプライアンス維持への取り組みについて (株式会社ZOZOテクノロジーズ) <br> 2. マルチアカウント運用の開始までの取り組み (株式会社ウェザーニューズ) <br> 3. 「進化し続けるインフラ」のためのマルチアカウント管理 (株式会社リクルート) => 約90の AWS アカウントに対して横断的な管理、コスト配賦、共通機能の提供などの運用について。|
|`---`| [【オンラインMeetup イベントレポート】第二回 AWSマルチアカウント事例祭り - ZOZO TECH BLOG](https://techblog.zozo.com/entry/20210209-meetup-report) / [`logmi  書き起こし`](https://logmi.jp/events/2551)| [`YouTube`](https://www.youtube.com/watch?v=LHVifH4P4GM)| 1. マルチアカウントでのIAMユーザ把握と可視化 IAMユーザー棚卸しへの取り組み (株式会社ZOZOテクノロジーズ) <br> 2. AWS導入から3年 AWSマルチアカウント管理で変わらなかったこと変えていったこと (ニフティ株式会社) <br> 3. セキュリティインシデントを乗り越えるために行ったマルチアカウントでの取り組みについて (Classi株式会社)|

## Network
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [AWS Summit Tokyo 2019 - 【初級】AWS を支えるグローバルネットワーク](https://pages.awscloud.com/rs/112-TZM-766/images/C1-02.pdf)| -| AWS のデータセンターやネットワークの物理構成と特徴やメリットについて。|
|`300`| [AWSネットワークの論理的な側面 ～ AWSのバックボーンネットワークに関するDeepな話（2） (1/4)：CodeZine（コードジン）](https://codezine.jp/article/detail/9790)| -| Mapping Service (マッピングサービス)を利用した VPC 内で仮想サーバー同士が通信可能な仕組みの解説。|
|`300`| [パケットの気持ちになって辿る Amazon VPC のルーティング - AWS Summit Online 2020](https://pages.awscloud.com/rs/112-TZM-766/images/AWS-08_AWS_Summit_Online_2020_NET01.pdf)| -| オンプレミスのルーター/スイッチの考え方とは異なる、VPC 内でのクラウドネットワーキングの感覚を掴む。|
|`300`| [「知らなくても困らないけど、知ると楽しいVPCの裏側の世界」というテーマでビデオセッションでお話ししました #devio2020 - DevelopersIO](https://dev.classmethod.jp/articles/devio-connect-2020-chibayuki-vpc/)| -| AWS Hyperplane や Blackfoot という VPC を裏側で支える技術について。 |
|`300`| [顧客拠点から Amazon VPCへの接続パターンまとめ (Whitepaper参照） - DevelopersIO](https://dev.classmethod.jp/articles/whitepaper-translate-jpn-vpc-connectivity-options-01/)| -| VGW, Direct Connect, Transit Gateway の利用パターンがまとまっている。|

## Security

### General - Security
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [クラウドセキュリティ - AWS](https://aws.amazon.com/jp/security/?nc=sn&loc=0)| -| AWS クラウドセキュリティに関するトップページ。[責任共有モデル](https://aws.amazon.com/jp/compliance/shared-responsibility-model/)、[AWS におけるデータ保護](https://aws.amazon.com/jp/compliance/data-protection/)、[AWS でのデータプライバシー](https://aws.amazon.com/jp/compliance/data-privacy/)、[その他 AWS クラウドセキュリティに関するリソースの一覧](https://aws.amazon.com/jp/products/security/resources/) などへのポータルになっている。|
|`100`| [AWS セキュリティドキュメント](https://docs.aws.amazon.com/ja_jp/security/)| -| AWS の各サービスのセキュリティに関する専用の章へのリンク一覧。|
|`200`| [ゼロトラストアーキテクチャ: AWS の視点 - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/zero-trust-architectures-an-aws-perspective/)| -| ゼロトラストの定義と指針など。|
|`200`| [脅威モデリングのアプローチ方法 - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/how-to-approach-threat-modeling/)| -| 具体的な方法ではないが、モデリングを進める上での段取りや考え方がまとめられている。|
|`200`| [NIST サイバーセキュリティ フレームワーク (CSF) - AWS クラウドにおける NIST CSF への準拠](https://d1.awsstatic.com/whitepapers/compliance/JP_Whitepapers/NIST_Cybersecurity_Framework_CSF_JP.pdf)| -| 2014年2月に米国国立標準研究所（NIST）が 1.0 版を公開した CSF（サイバーセキュリティフレームワーク）はサイバーセキュリティの推奨ベースラインとなっており、NIST CSF のコアを支え、セキュリティ対策 (サブカテゴリ) の達成を可能にする AWS のソリューションと機能について記載したホワイトペーパー。NIST CSF については [IPA が出している翻訳](https://www.ipa.go.jp/files/000071204.pdf) はあるが、[【解説】NIST サイバーセキュリティフレームワークの実践的な使い方 - NRIセキュア](https://www.nri-secure.co.jp/blog/nist-cybersecurity-framework) がわかりやすく概要がまとまっている。|

### Application - Security
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [AWS における安全な Web アプリケーションの作り方 - AWS Summit Online 2021](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-55_AWS_Summit_Online_2021_Developing-Secure-Web-Applications-on-AWS.pdf)| [`Youtube`](https://youtu.be/TxBg7FWMAUA)| IPA の「安全なウェブサイトの作り⽅」や OWASP Top 10 に沿った考え方が記載されている。|
|`300`| [2020年版 チーム内勉強会資料その1 : JSON Web Token - r-weblife](https://ritou.hatenablog.com/entry/2020/06/08/050000)| -| Cognito でも利用されている JSON Web Token(JWT) について。|

### Audit & Compliance - Security
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [責任共有モデルとは何か、を改めて考える - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/rethinksharedresponsibility/)| -| AWSがホストオペレーティングシステムと仮想化レイヤーから、サービスが運用されている施設の物理的なセキュリティに至るまでの要素をAWSが運用、管理、および制御することから、お客様の運用上の負担を軽減するために役立つ、責任共有モデルのモデルの考え方や実際のビジネスへの適用方法について理解のポイント。|
|`100`| [アマゾンウェブサービス: リスクとコンプライアンス - AWS Whitepaper](https://d1.awsstatic.com/whitepapers/compliance/JP_Whitepapers/AWS_Risk_and_Compliance_Whitepaper_JP.pdf)| -| AWS のお客様が IT 環境をサポートする既存の統制フレームワークに AWS を統合する際に役立つ情報を提供するドキュメント。AWS 統制の評価に関する基本的なアプローチについて説明し、統制環境の統合の際に役立つ情報を提供したり、クラウドコンピューティングのコンプライアンスに関する一般的な質問について、AWS 固有の情報を掲載している。|
|`100`| [AWS セキュリティ監査のガイドライン - AWS 全般のリファレンス](https://docs.aws.amazon.com/ja_jp/general/latest/gr/aws-security-audit-guide.html)| -| 基本的なことではあるが、監査を実践するためのガイドラインが羅列されている。|

### AWS Account - Security
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [(私のように)セキュリティを何から始めれば良いか分からない開発者の方へ - AWS Builders Online Series 2022](https://pages.awscloud.com/rs/112-TZM-766/images/BOS32_AWS-Builders-Online-Series_2022-Q1_Presentation-Deck.pdf)| [AWS](https://resources.awscloud.com/aws-builders-online-series-japanese/bos32)| クラウドとそのサービスが提供する機能を活用して、セキュリティも自動化しながら、前向きに向き合っていくためのヒントなど。|
|`200`| [AWS アカウントを守るためにおさえておきたいセキュリティ対策 - AWS Summit Online 2021](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-52_AWS_Summit_Online_2021_Security_measures_you_should_keep_in_mind_to_protect_your_AWS_account.pdf) | [`Youtube`](https://youtu.be/nxfMzXTaCVw) | AWS Well-Architected フレームワーク セキュリティの柱に沿った AWS アカウントを守るために実施すべきセキュリティ対策。|
|`200`| [AWSの異常課金で気付いた不正アクセス--インシデントにどう対応したのか - ZDNet Japan](https://japan.zdnet.com/article/35133681/)| -| 初動対応の調査や、社内の対応体制と外部連携についてなど。|
|`300`| [AWS セキュリティリファレンスアーキテクチャ (AWS SRA) - AWS 規範的ガイダンス](https://docs.aws.amazon.com/ja_jp/prescriptive-guidance/latest/security-reference-architecture/welcome.html)| -| マルチアカウント環境において AWS セキュリティサービスの完全補完をデプロイするための包括的なガイドラインセット。AWS セキュリティサービスを AWS ベストプラクティスに沿うように設計、実装、および管理するために利用するためのドキュメント。|
|`300`| [AWS環境にセキュアなベースラインを提供するテンプレート「Baseline Environment on AWS」のご紹介 - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/announcing-baseline-environment-on-aws/)| -| AWS Japanのソリューションアーキテクトが AWS Samples に公開している BLEA についての紹介。CDK をベースにした AWS のセキュリティのベストプラクティスを実装した環境を、迅速に実現するためのテンプレート。単一のアカウントでも、また AWS Control Tower によるマルチアカウント環境でも同じように利用可能。|

### Network - Security
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`200`| [AWS におけるネットワーク＆アプリケーション保護のすすめ - AWS Summit Online 2021](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-38_AWS_Summit_Online_2021_SEC02.pdf) | [`Youtube`](https://youtu.be/PSTjZ_g-bNo)| AWS Network Firewall, AWS WAF,AWS Shield Advanced を利用した境界防御のパターンが一般的な構成、サーバーレス、遅延にセンシティブな場合、オンプレの組み合わせなど紹介されている。|
|`200`| [AWS 環境における脅威検知と対応 - AWS Summit Online 2021](https://d1.awsstatic.com/events/jp/2021/summit-online/AWS-39_AWS_Summit_Online_2021_SEC03.pdf)| [`Youtube`](https://youtu.be/VWp6OAxPbRc)| Amazon GuardDuty、AWS Security Hub、Amazon Detective による脅威を検知、監視、調査について。|
|`300`| [DDoS に対する AWS のベストプラクティス（英語）](https://d1.awsstatic.com/whitepapers/Security/DDoS_White_Paper.pdf)| -| DDoS 攻撃に対する回復力のあるアプリケーションを構築するための規範的な DDoS ガイダンス。ボリューム型攻撃やアプリケーション層に対する攻撃など、さまざまな攻撃タイプの紹介と各攻撃タイプを管理する上で最も効果的なベストプラクティスの説明。DDoS 緩和戦略に適合するサービスや機能および、それぞれがどのようにアプリケーションを保護するのに役立つのかについての要点など。|
|`300`| [インターネットからのイングレストラフィックフローのためのファイアウォールのデプロイ設計 - Amazon Web Services ブログ](https://aws.amazon.com/jp/blogs/news/design-your-firewall-deployment-for-internet-ingress-traffic-flows/)| -| AWS WAF, AWS Network Firewall, Gateway Load Balance, ELB Sandwich(ELB + サードパーティアプライアンスの EC2) それぞれのアーキテクチャ図と特徴の一覧表によるまとめ。|

### Vulnerabilities - Security
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [セキュリティツールの評価は難しい - knqyf263's blog](https://knqyf263.hatenablog.com/entry/2022/03/15/064819)| -| AWS 関係なく、セキュリティツールを利用するにあたって、検知数が多い少ないで良し悪しを判断しがちになってしまうという話。|
|`100`| [脆弱性ハンドリングと耐える設計 -Vulnerability Response-](https://www.slideshare.net/nakatomoorg/vulnerability-response)| -| 脆弱性情報を収集、トリアージ（取捨選択）、対処し、攻撃の被害から防ぐための基礎的な内容。|

## Serverless (サーバーレス)
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [サーバーレスコンピューティング - ユースケース別クラウドソリューション - AWS](https://aws.amazon.com/jp/serverless/)| -| AWS でのサーバーレスとは？について。[こちらの「なぜサーバーレスアプリケーションを構築するのですか?」](https://aws.amazon.com/jp/serverless/build-a-web-app/)という部分に主なメリットがまとめられている。|
|`200`| [形で考えるサーバーレス設計 / サーバーレスパターン - AWS](https://aws.amazon.com/jp/serverless/patterns/serverless-pattern/)| -| サーバーレスの組み合わせの代表的な適用シーン/ユースケースと実装形。|
|`300`| [今日から始める、サーバーレス Well-Architected Framework - Speaker Deck](https://speakerdeck.com/_kensh/serverless-well-architected-framework)| -| Well-Architected フレームワークに則った設計をするための具体例。|
|`300`| [Serverless Land - Resources for learning about AWS serverless technology](https://serverlessland.com/)| -| サーバーレスの設計パターンなど。|
|`---`| [物流支援サービスを支えるAWSサーバーレスアーキテクチャ戦略 - ZOZO TECH BLOG](https://techblog.zozo.com/entry/aws-serverless-architecture-strategy)| -| 自社ECサイト間でリアルタイムに在庫情報を連携する仕組みでサーバーレスを活用。|
|`---`| [AWS 導入事例：株式会社 日立製作所 - AWS](https://aws.amazon.com/jp/solutions/case-studies/hitachi-serverless/)| -| 1,000 万台超の自動車へ更新ソフトウェアを配信する OTA サービスをサーバーレスで移行を検討し、運用負荷も大幅に軽減できるという試算。|
|`---`| [AWS 導入事例：ヤマハ発動機株式会社 - AWS](https://aws.amazon.com/jp/solutions/case-studies/yamaha-nri/)| -| POS システムをサーバーレスのクラウドネイティブアーキテクチャで構築し、わずか 3 ヶ月で実装。システムの構築コストはバックエンドの構築費用がほぼゼロだったため当初見込んだ開発予算よりも抑えられた。さらに、サーバーレスのマイクロサービスとしてシステム構築することで、短期間かつ低コストでの開発を実現。システム全体の可用性と信頼性を向上させるとともに、拡張性と保守性の向上も可能に。|

## Storage
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [5分で絶対に分かるオブジェクトストレージ：5分で絶対に分かる（3/5 ページ） - ＠IT](https://atmarkit.itmedia.co.jp/ait/articles/1705/29/news014_3.html)| -| オブジェクトストレージとファイルストレージの違いを「場所を自分で把握する必要があるかどうか」という観点で、駐車場の例で説明している。|
|`100`| [ストレージの勉強方法を聞いてみた。 - 変化を求めるデベロッパーを応援するウェブマガジン](https://aws.amazon.com/jp/builders-flash/202110/way-to-learn-storage/)| -| おすすめの資料や書籍なども。|
|`200`| [Comparing your on-premises storage patterns with AWS Storage services - AWS Storage Blog (English)](https://aws.amazon.com/blogs/storage/comparing-your-on-premises-storage-patterns-with-aws-storage-services/)| -| オンプレミスのストレージの考え方と、 AWS でのストレージの考え方。|
|`200`| AWS Storage - EBS vs S3 vs EFS| [`YouTube`](https://www.youtube.com/watch?v=6vNC_BCqFmI)| [ここから](https://youtu.be/6vNC_BCqFmI?t=238) EBS, S3, EFS の違いがわかりやすく解説されている。|

## Test
|Lv.|タイトル|動画URL|備考|
|---|---|---|---|
|`100`| [テストポリシー - Amazon EC2](https://aws.amazon.com/jp/ec2/testing/?nc1=h_ls)| -| ネットワーク負荷テストを実施する場合に一読しておくドキュメント。|
|`100`| [ペネトレーションテスト（侵入テスト）- AWS セキュリティ](https://aws.amazon.com/jp/security/penetration-testing/)| -| AWS インフラストラクチャに対するセキュリティ評価または侵入テストの実施ポリシー。|
|`200`| [AWS での分散負荷テスト - AWS ソリューション](https://aws.amazon.com/jp/solutions/implementations/distributed-load-testing-on-aws/)| -| 大規模および負荷時のソフトウェアアプリケーションテストを自動化して、リリース前に性能上の潜在的なパフォーマンスの問題を特定するのに役立つツールを AWS サービスで構築できる。[大規模な負荷テストを実行可能。「Distributed Load Testing on AWS」 を試してみる - builders.flash☆](https://aws.amazon.com/jp/builders-flash/202108/distributed-load-testing/) に、このソリューションを実施した結果画面があるのでこちらも参考にどうぞ。|
|`200`| [AWSでカオスエンジニアリング！ AWS Fault Injection Simulatorが利用可能になりました - DevelopersIO](https://dev.classmethod.jp/articles/aws-fault-injection-simulator-ga/)| -| フォールトインジェクション実験の目的や、AWS で実施するサービスの紹介。|
|`200`| [AWS Lambda Power Tuningによる関数のプロファイリング](https://aws.amazon.com/jp/blogs/news/operating-lambda-performance-optimization-part-2/)| -| [AWS Lambda Power Tuning](https://github.com/alexcasalboni/aws-lambda-power-tuning) を利用した、最適な割り当てメモリを計測できるツールが紹介されている。|
|`300`| [イチから理解するサーバーレスアプリケーション - 開発サーバーレス開発環境とテスト](https://pages.awscloud.com/rs/112-TZM-766/images/20200827_serverless_session2.pdf)| -| [テストしやすい Lambda 関数の書き方](https://pages.awscloud.com/rs/112-TZM-766/images/20200827_serverless_session2.pdf#page=56)や、[AWSのサービスを利⽤するコードのUnit Test](https://pages.awscloud.com/rs/112-TZM-766/images/20200827_serverless_session2.pdf#page=73)の方法論など。|
|`300`| [2021年版、サーバーレスのテスト手法を考える / Serverless Testing 2021 - Speaker Deck](https://speakerdeck.com/_kensh/serverless-testing-2021)| -| 外部リソースを含むテスト、後半なスタックで構成されたビジネスロジック、非同期の副作用を伴うテストなど。|
