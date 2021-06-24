
### プロジェクトの作成
```sh
docker-compose run --rm web-back sh -c "django-admin startproject config ."
```

### アプリの作成
```sh
docker-compose run --rm web-back sh -c "python manage.py startapp todo"
```

### ビルド
```sh
docker-compose up --build
```

### マイグレートファイルの作成
```sh
docker-compose run --rm web-back sh -c "python manage.py makemigrations"
```

### マイグレート
```sh
docker-compose run --rm web-back sh -c "python manage.py migrate"
```

### スーパーユーザーの作成
```sh
docker-compose run --rm web-back sh -c "python manage.py createsuperuser"
# 初期
example@gmail.com
password
```

### 静的ファイルをまとめる
```sh
docker-compose run --rm web-back sh -c "python manage.py collectstatic"
```

### mysqlへ接続
```sh
docker exec -it container_db bash
```

### テストの実行
```sh
docker-compose run --rm web-back sh -c "python manage.py test"
```

### reactプロジェクト作成
```sh
docker-compose run --rm web-front sh -c "npx create-react-app ."
```

### next.jsに必要なモジュールのインストール
```sh
docker-compose run --rm web-front sh -c "yarn add next axios"
docker-compose run --rm web-front sh -c "yarn add --dev typescript @types/react"
```

### localhostにアクセスする

