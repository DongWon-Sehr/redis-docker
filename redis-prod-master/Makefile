shell:
	docker-compose run --service-ports web bash

build: clean
	docker-compose build

up:
	docker-compose up

up-d:
	docker-compose up -d

down:
	docker-compose down --remove-orphans

clean: down
	find . -type d -name 'redis-data' -exec rm -fr {} +
	find . -type d -name 'redis-log' -exec rm -fr {} +

clean-up: clean
	docker-compose up