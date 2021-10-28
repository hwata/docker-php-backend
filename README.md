# docker-php-backend

phpのバックエンド（LaravelやCakePHP）を動かすためのDockerサンプル

## 起動方法
```bash
docker-compose up -d
```
## 終了方法
```bash
docker-compose down
```
## APPサーバーへのログイン
```bash
docker-compose exec app bash
```
## Laravel8.x

nginx/default.conf で公開ディレクトリを以下に変更する

root /var/www/html/public;
```bash
docker-compose up -d
docker-compose exec app bash
rm .gitkeep
composer create-project laravel/laravel .
```

## CakePHP4.x インストール

nginx/default.conf で公開ディレクトリを以下に変更する

root /var/www/html/webroot;

```bash
docker-compose up -d
docker-compose exec app bash
rm .gitkeep
composer create-project --prefer-dist cakephp/app:4.* .
```

# Author
 
* 作成者 hwata
* 所属 http://www.codelab.jp/

 
# License

This is under [MIT license](https://en.wikipedia.org/wiki/MIT_License).
