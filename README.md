
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

