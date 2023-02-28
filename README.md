
### Step by Step
Clone Repository
```sh
git clone https://github.com/denissabiao/laravel-docker-setup.git
```

Clone Laravel Files
```sh
git clone https://github.com/laravel/laravel.git app-laravel
```

Copy docker-compose.yml, Dockerfile and docker/ directory files to your project
```sh
cp -rf setup-docker-laravel/* app-laravel/
```
```sh
cd app-laravel/
```


Create .env File
```sh
cp .env.example .env
```



Start project containers
```sh
docker-compose up -d
```


Access the container
```sh
docker-compose exec app bash
```


Install project dependencies
```sh
composer install
```


Generate Laravel project key
```sh
php artisan key:generate
```


Access the project
[http://localhost:8188](http://localhost:8188)
