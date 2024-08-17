# Docker環境構築

## セットアップ手順
1. Docker と Docker Compose がインストールされていることを確認してください。
2. リポジトリをクローンまたはダウンロードします。
3. .env.exampleをコピーして、.envのファイルを作り編集する
```
# postgres
POSTGRES_USER=postgres                 # postgresを変更する
POSTGRES_PASSWORD=postgres             # postgresを変更する
POSTGRES_DB=sns-udemy                  # sns-udemyを変更する

# pgadmin
PGADMIN_DEFAULT_EMAIL=admin@admin.com  # admin@admin.comを変更する
PGADMIN_DEFAULT_PASSWORD=admin         # adminを変更する
```
4. Docker コンテナをビルドし、バックグラウンドで実行します。
```
docker-compose up -d --build
```

## ブラウザでのアクセス
1. `http://localhost:8080` にアクセスして pgAdmin のページが表示されることを確認します。
