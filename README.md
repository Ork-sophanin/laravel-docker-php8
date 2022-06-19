## Setup Guide

### Without Docker

- Create .env file with two commands `cd source_code/`, `cp .env.example .env` and replace with your own env variables.
- `composer install`
- `php artisan serve` (You will be exposed through url: `http://127.0.0.1:8000`)

### With Docker
Run the following scripts for UNIX (Mac, Linux):
```bash
$ cd source_code/
$ composer install
$ cp .env.example up -d
$ docker-compose up -d
```
DOS(Windows):
```bash
$ cd source_code/
$ composer install
$ copy .env.example .env
$ docker-compose up -d
```

## Available Services with Docker Container
Once you managed to run the docker container, the following services will be available:
- Nginx will serve as a reverse proxy and will be exposed through port 80 (http://localhost)
- Database (Mysql) (Host: 127.0.0.1, Port: 3306)
- PhpMyAdmin (Mysql) (http://localhost:9001)
