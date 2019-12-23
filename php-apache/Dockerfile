
FROM php:7.2.1-apache
MAINTAINER egidio docile
RUN apt-get update && apt-get install -y \
    zlib1g-dev \
    libzip-dev
RUN docker-php-ext-install pdo pdo_mysql mysqli zip
RUN pecl install xdebug; \
docker-php-ext-enable xdebug

RUN a2enmod rewrite