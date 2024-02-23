
## 環境構築参考サイト
- [Laravel9とVue.jsをDockerで導入してみよう!](https://zenn.dev/eguchi244_dev/articles/laravel-vue-docker-introduction-20230828)
- [Laravel9のVite環境でVue.js 3を利用する方法](https://reffect.co.jp/laravel/laravel9_vite)

## 環境構築後の操作
- dockerイメージとコンテナの作成
```
docker compose build --no-cache && docker-compose up -d
```

- phpコンテナにログイン
```
docker-compose exec php bash
```

- nodeコンテナにログイン&開発サーバーを起動
```
docker-compose exec node /bin/sh
cd /var/www/diary-app
npm run dev
```

### リファレンス
- [docker-composeコマンド概要](https://docs.docker.jp/v1.12/compose/reference/overview.html)

### バージョン情報

name|version
--|--
PHP | 8.0.30
Laravel | 9.52.16