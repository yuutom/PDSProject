# APIに関する基本設計書
APIは以下の二つにカテゴライズする。
* 公開API
* 非公開API

# ドキュメント
API仕様書は以下の2つの形式で参照する想定
1. OpenAPI
2. redoc

# 編集
API仕様書の編集はVSCodeにて行う想定

# API仕様書作成環境構築
1. Python3をインストール
2. VSCodeをインストール
3. VSCodeの拡張機能で以下をインストールする
* Japanese Langage
* Python
* autoDocstring - Python Docstring Generator
* Node.jsをインストール
* OpenAPI(Swagger) Editor
* openapi-designer
* Prettier - Code Formatter
4. PowerShellを管理者として起動し、以下のコマンドを実行
```
PowerShell Set-ExecutionPolicy RemoteSigned
```
5. VSCodeでopenapi.yamlを開く
6. 右クリック→コマンドパレット→OpenApi Designer: Previewを選択 → OpenAPIでドキュメントを閲覧できる
7. VSCodeのターミナルで以下のコマンドを実行する
```
npm install -g redoc-cli
```
8. VSCodeのターミナルで以下のコマンドを実行する
```
redoc-cli bundle ./openapi.yaml --output ./openapi.html
```
9. openapi.htmlが同階層に出力されるのでブラウザで開く → redoc形式のドキュメントを閲覧できる