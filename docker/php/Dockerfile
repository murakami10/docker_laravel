FROM php:7.3-fpm
COPY php.ini /usr/local/etc/php

RUN apt-get update
RUN docker-php-ext-install bcmath pdo_mysql