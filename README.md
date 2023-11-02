## Running
docker run --rm -v "$(pwd)":/app composer install

docker-compose up
docker-compose exec app php artisan key:generate
docker-compose exec app php artisan optimize


