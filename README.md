# Set up Laravel with Docker


こちらのリポジトリを、cloneします。
```
$ git clone https://github.com:Mitsuya-Sora/set_up_laravel_with_docker
```
```
$ cd set_up_laravel_with_docker
$ docker-compose up -d --build
$ docker-compose exec app bash
$ composer install
$ cp .env.example .env
$ php artisan key:generate
$ php artisan migrate
```
[http://127.0.0.1:10080](http://127.0.0.1:10080)にアクセスします。
