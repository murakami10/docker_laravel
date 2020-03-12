FROM php:7.2

WORKDIR /tmp

RUN apt-get update -y \
    && apt-get install -y git unzip
RUN curl -sS https://getcomposer.org/installer | php \
    && mv composer.phar /usr/local/bin/composer
RUN composer self-update
RUN mkdir /src

WORKDIR /src
ENTRYPOINT ["composer"]
