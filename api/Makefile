run-api:
	cp ./src/.env.example ./src/.env
	docker compose build
	docker compose up -d
	docker exec php /bin/sh -c "composer install && chmod -R 777 storage && php artisan key:generate && php artisan migrate:fresh --seed"

run-api-tests:
	docker exec php /bin/sh -c "php artisan test"

kill-api:
	docker compose down