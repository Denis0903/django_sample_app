# django_sample_app

English 1st,Japanese 2nd.

# Prerequisites

- Construction of environment for pyenv and pipenv
- Pyenv has python3.7 installed and ready to use

# Environment

- When you run "pipenv install Django" under the root directory, the related modules listed in the pipfile will be installed.

# Execution method

- Start virtual environment with "pipenv shell"
- Register an arbitrary character string in DJANGO_APP_SECRET_KEY in the environment variable of the environment where the Django app is deployed (Because it is a Secret Key used in Django, keep a long character string secret like a password)
- Go to mybook directory and run "python manage.py runserver"
- When you access the right page, you will be taken to the administration screen (ID: admin Password: adminpassword) (Needless to say, Chrome is recommended.) Http://127.0.0.1:8888/admin
- When you access the page on the right, you will be taken to the application screen (not to mention Chrome is recommended) http://127.0.0.1:8000/cms/book/

# Description of each folder

- mybook
  - The whole module of the Django application
- cms in mybook
  - In mybook, a folder that serves as a sample app
- mybook in mybook
  - Folder that manages application setting information in mybook

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
