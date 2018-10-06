# initial
$ git clone https://github.com/naoki0531/template-laravel.git
$ cd template-laravel
$ git submodule init
$ git submodule update
$ git submodule add {source repository} src
$ cp .env.laradock laradock/.env
$ cd laradock
$ docker-compose up -d --build nginx mysql workspace
$ docker-compose exec workspace composer install
$ docker-compose exec workspace npm install
$ docker-compose exec workspace php artisan key:generate

http://localhost:8080/