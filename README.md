# Set up Laravel with Docker
Docker,Dockerをインストールします。

https://docs.docker.com/docker-for-windows/install

https://docs.docker.com/docker-for-mac/install

こちらのリポジトリを、cloneします。
```
$ git clone git@github.com:Mitsuya-Sora/set_up_laravel_with_docker.git
```
コンテナを起動し、初期設定をします。
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
