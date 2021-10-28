# docker-php-backend

起動
docker-compose up -d

APPサーバーへのログイン
docker-compose exec app bash

Laravel8.x
nginx/default.conf
公開ディレクトリを以下に変更する
root /var/www/html/public;


composer create-project laravel/laravel .



CakePHP4.x インストール
nginx/default.conf
公開ディレクトリを以下に変更する
root /var/www/html/webroot;

docker-compose up -d
docker-compose exec app bash
rm .gitkeep
composer create-project --prefer-dist cakephp/app:4.* .

