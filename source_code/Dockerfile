FROM php:8.0-fpm

RUN apt-get update -y && apt-get install -y openssl libzip-dev zip unzip git curl

RUN docker-php-ext-install zip mysqli bcmath ctype fileinfo pdo pdo_mysql tokenizer

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin/ --filename=composer
