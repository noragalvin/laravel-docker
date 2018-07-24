
[Simple, fast routing engine](https://laravel.com/docs/routing).
## Docker service

- nginx
- php

## How to run
- Install [docker](https://docs.docker.com/install/).
- Install [docker composer](https://docs.docker.com/compose/install/)
- Run
```
docker run --rm -v $(pwd):/app composer/composer install
```
- Run
```
docker-compose up
```
- Run
```
cp .env.example .env
```
- Run
```
docker-compose exec app php artisan key:generate
docker-compose exec app php artisan optimize
```
- Final step. Run
```
docker-compose up
```
- The application will now be ready to use go ahead and hit http://localhost in your browser and you’ll presented with this lovely screen.
![](https://cdn-images-1.medium.com/max/800/1*4MleKBjK5aU_rL4fs1ro8g.png)