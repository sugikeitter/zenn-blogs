---
title: "Boto3の設定あれこれ（profile名、アクセスキー、Config、ログの設定とか）"
emoji: "🧑‍💻"
type: "tech" # tech: 技術記事 / idea: アイデア
topics: ["aws", "python", "プログラミング", "boto3"]
published: true
---

# はじめに
ローカル環境でBoto3を利用する時にコード内でprofile名を指定したり、アクセスキーを埋め込むことがある。それ以外にBoto3利用時にはConfigやログ出力を設定することもでき、こちらは開発環境や本番環境でも活用できる。これらの設定は[公式ドキュメント](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html)に記載されているがそれぞれ別のページに記載されているため、自分が一覧で見やすいようこの記事にまとめた(ง •̀_•́)ง

Boto3自体を詳しく知りたい場合は、以下の記事も読んでみてください。
https://zenn.dev/sugikeitter/articles/6648845968cec6

# Sessionについて
https://boto3.amazonaws.com/v1/documentation/api/latest/reference/core/session.html

AWSのAPIを利用するメソッドを持つ`Client/Resource`オブジェクトは、`boto3.client('AWS_SERVICE_NAME')`や`boto3.resource('AWS_SERVICE_NAME')`を利用して生成できるが、この時の引数にいくつか設定を指定することができる。

```python
import boto3
s3_client = boto3.client('s3') # Clientオブジェクト生成
s3_resource = boto3.resource('s3') # Resourceオブジェクト生成
```

これらの`client()/resource()`メソッドは、内部的には`Session`オブジェクトの`client()/resource()`メソッドを利用している。そのため`Session`オブジェクトを生成する時にBoto3の設定をして、そこから`Client/Resource`オブジェクトを生成することもできる。

ちなみに公式ドキュメントでは`Session`オブジェクトを生成するコードとして、`boto3.Session()`を[利用している場面](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html#passing-credentials-as-parameters)と、`boto3.session.Session()`を[利用している場面](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/session.html#custom-session)とが混ざっていてややこしいので個人的な補足をしておく。（以下の2パターンがある）

```python
import boto3
my_session = boto3.Session()
s3_client = my_session.client('s3') # Clientオブジェクト生成
ddb_resource = my_session.resource('dynamodb') # Resourceオブジェクト生成
```

```python
import boto3.session
my_session = boto3.session.Session()
s3_client = my_session.client('s3') # Clientオブジェクト生成
ddb_resource = my_session.resource('dynamodb') # Resourceオブジェクト生成
```

上のどちらを利用しても生成されるのは同じ`boto3.session.Session`オブジェクトであるため、
記述量が短いの`boto3.Session()`を使えば良いと思う。
なぜ同じなのに短い記述で済むかと言うと、`boto3`パッケージのルート階層の`__init__.py`で`from boto3.session import Session`をしているためである。


# コード内でprofile名の指定
https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html#shared-credentials-file

まずは一番よく使う（と思う）名前付きprofileの指定方法について。
こちらは`client()/resource()`メソッドでは指定できないので、`Session`オブジェクト生成時にprofile名を指定する必要がある。

```python
import boto3
my_session = boto3.Session(profile_name='YOUR_PROFILE_NAME')
s3_client = my_session.client('s3') # Clientオブジェクト生成
ddb_resource = my_session.resource('dynamodb') # Resourceオブジェクト生成
```

SDKとは関係なく、profileの設定ではIAMユーザーのアクセスキーだけでなく`role_arn`と`source_profile`を利用してIAMロールの利用も可能。
https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-role.html

# コード内でアクセスキーの埋め込み
https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html#passing-credentials-as-parameters

コード内で直接アクセスキーを埋め込むことも可能。
この場合はprofile名の指定と異なり`client()/resource()`メソッドでの指定と`Session`オブジェクト生成時での指定のどちらも可能。

- `client()/resource()`メソッドでの指定
```python
import boto3
# Clientオブジェクト生成
s3_client = boto3.client(
    's3',
    aws_access_key_id='YOUR_ACCESS_KEY',
    aws_secret_access_key='YOUR_SECRET_KEY',
    aws_session_token='YOUR_SESSION_TOKEN' # IAMロール利用の場合のみ設定
)
# Resourceオブジェクト生成
s3_resource = boto3.resource(
    's3',
    aws_access_key_id='YOUR_ACCESS_KEY',
    aws_secret_access_key='YOUR_SECRET_KEY',
    aws_session_token='YOUR_SESSION_TOKEN' # IAMロール利用の場合のみ設定
)
```

- `Session`オブジェクト生成時での指定

同じ設定から複数の`Client/Resource`オブジェクトを利用したい場合は、一度Sessionを生成してからの方が記述量が少なくて済む。
```python
import boto3

my_session = boto3.Session(
    aws_access_key_id='YOUR_ACCESS_KEY',
    aws_secret_access_key='YOUR_SECRET_KEY',
    aws_session_token='YOUR_SESSION_TOKEN' # IAMロール利用の場合のみ設定
)
# Client/Resourceオブジェクトの生成
s3_client = my_session.client('s3')
s3_resource = my_session.resource('s3')
ddb_client = my_session.client('dynamodb')
```

# AssumeRoleで取得した一時的な認証情報の埋め込み
https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.assume_role

IAMロールを利用したい場合はSTSのAssumeRoleで一時的な認証情報を取得して、上で紹介したコード内にアクセスキーを埋め込む合わせ技でも可能。

```python
import boto3
# AssumeRoleで一時的な認証情報を取得
sts_client = boto3.client('sts')
temp_creds = sts_client.assume_role(
    RoleArn='arn:aws:iam::123456789:role/YOUR_ROLE_NAME', # IAMロールのARN
    RoleSessionName='YOUR_ROLE_SESSION_NAME', # 識別できる名前
    DurationSeconds=1800 # 有効期限
)
# 一時的な認証情報を利用してClient/Resourceオブジェクトの生成
s3_client = boto3.client(
    's3',
    aws_access_key_id=temp_creds.get('Credentials').get('AccessKeyId'),
    aws_secret_access_key=temp_creds.get('Credentials').get('SecretAccessKey'),
    aws_session_token=temp_creds.get('Credentials').get('SessionToken')
)
```

# Configの指定
https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html

Configを利用するとREST APIの挙動に関わる設定が可能。Configが利用できるのは`client()/resource()`メソッドのみ。

個人的に一番利用する機会が多そうな設定は、SDK内でのREST APIのリトライ回数かなと思う。
[公式ドキュメントにも記載されているが](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/retries.html)、Boto3で何も指定しない場合のリトライ処理はLegacyモードという、他の言語のSDKとリトライ対象のHTTPステータスコードなどが異なるものになるため注意。
> Legacy mode is the default mode used by any Boto3 client you create. As its name implies, legacy mode uses an older (v1) retry handler that has limited functionality.

他言語のデフォルトと合わせるためにはConfigで`retries`をStandardモードに指定する必要がある。

> Standard mode is a retry mode that was introduced with the updated retry handler (v2). This mode is a standardization of retry logic and behavior that is consistent with other AWS SDKs.

```python
import boto3
# リトライをStandardモードに設定
s3_client = boto3.client('s3', config=Config(retries={'mode': 'standard'}))
ddb_resource = my_session.resource('dynamodb', config=Config(retries={'mode': 'standard'}))
```

他にもConfigで指定できるのはいくつかあるが、だいたいはデフォルト値で大きな問題はでない気がする。
ただ、性能や負荷をチューニングしたい場合に触るかもしれない項目を以下に挙げておく。

```python
import boto3
# HTTPクライアントの接続に関わる設定を指定する例
s3_client = boto3.client(
    's3',
    config=Config(
        connect_timeout=30, # DEFAULT 60
        read_timeout=15, # DEFAULT 60
        max_pool_connections=20  # DEFAULT 10
    ))
```

# ログの設定

https://boto3.amazonaws.com/v1/documentation/api/latest/reference/core/boto3.html

`boto3`, `botocore`パッケージ内のコードで出力するログのレベルを変更でき、開発時の調査やデバッグの時に便利。

```python
import boto3

# デフォルトだとboto3パッケージが対象で、ログレベルはDEBUGになる
boto3.set_stream_logger()

# boto3/botocoreのパッケージの細かい指定まで可能、ログレベルも変更可能
boto3.set_stream_logger('boto3.resources', logging.WARN)

# パッケージ指定を''にするとboto3/botocore全てのログが出るが、botocoreはcredential情報なども出るので本番環境などでは使わないように注意
boto3.set_stream_logger('')
```

特に調査に利用できそうなログが出るパッケージはこのへん。

| パッケージ名 | ログレベル | 出力内容 |
|------------|-----------|--------|
| `'botocore.endpoint'` | DEBUG | リクエスト時のヘッダやパラメーター（ヘッダに含まれる認証情報も出力されるので注意）|
|`'botocore.parsers'` | DEBUG | HTTPレスポンスボディ |


# リージョンの指定
リージョンの設定は、ややこしいことに以下のいろんなところで指定ができる。

- `client()/resource()`メソッド
```python
import boto3
# Clientオブジェクト生成時にリージョンを指定
s3_client = boto3.client('s3', region_name='YOUR_REGION')
# Resourceオブジェクト生成時にリージョンを指定
s3_resource = boto3.resource('s3', region_name='YOUR_REGION')
```

- `Session`オブジェクト
```python
import boto3
# Sessionオブジェクト生成時にリージョンを指定
my_session = boto3.Session(region_name='YOUR_REGION')
```

- Config利用
```python
import boto3
# Clientオブジェクト生成時にConfigを利用してリージョンを指定
s3_client = boto3.client('s3', config=Config(region_name='YOUR_REGION'))
# Resourceオブジェクト生成時にConfigを利用してリージョンを指定
s3_resource = boto3.resource('s3', config=Config(region_name='YOUR_REGION'))
```

# まとめ
Boto3を使ってコードを書く時に便利な情報を1ページでまとめることができた😎