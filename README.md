
# お問い合わせフォーム

## 環境構築
・Dockerビルド 
1. `git clone git@github.com:coachtech-material/laravel-docker-template.git`
2. `docker-compose up -d --build`

・Laravelビルド
1. `docker-compose exec php bash`
2. `composer install`
3. `cp .env.example .env`　にて、環境変数を変更。
- DB_HOST=127.0.0.1   ->  DB_HOST=mysql
- DB_DATABASE=laravel ->  DB_DATABASE=laravel_db
- DB_USERNAME=root    ->  DB_USERNAME=laravel_user
- DB_PASSWORD=        ->  DB_PASSWORD=laravel_pass
4. `php artisan key:generate`
5. `php srtisan migrate`
6. `php artisan db:seed`

## 使用技術(実行環境)
- Laravel  8.83.8
- PHP 7.4.9
- MySQL 15.1

## ER図
![sample](https://github.com/AgatsumaT/check-test/assets/149846646/89b4d53a-06f1-4ed4-a35f-4d93b161a55e)



## URL
- 開発環境：http://localhost/
- phpMyAdmin：http://localhost:8080/
