# django_sample_app

# 前提条件

- pyenvとpipenvの環境構築
- pyenvでpython3.7をインストールして利用できる状態にしていること

# 環境構築

- pipenv install Djangoをルートディレクトリ配下で実行するとpipfileに記載している関連モジュールがインストールされる

# 実行方法

- pipenv shell で仮想環境を起動
- Djangoアプリを展開する環境の環境変数において、DJANGO_APP_SECRET_KEYに任意の文字列を登録しておくこと（Djangoで利用するSecretKeyのためパスワード同様に長い文字列を秘密に管理しておくこと。）
- mybookディレクトリに移動し、python manage.py runserverを実施する
- 右記へアクセスすると、管理画面へ(ID:admin Password:adminpassword )（言わずもがな、Chromeがおすすめです。）　http://127.0.0.1:8888/admin
- 右記へアクセスすると、アプリケーション画面へ（言わずもがな、Chromeがおすすめです。）　http://127.0.0.1:8000/cms/book/

# 各フォルダの説明

- mybook
  - Djangoアプリケーションの全体モジュール
- cms in mybook
  - mybook内において、サンプルのアプリとなるフォルダ
- mybook in mybook
  - mybook内において、アプリケーションの設定情報を管理するフォルダ
