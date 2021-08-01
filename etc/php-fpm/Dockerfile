FROM php:7.4-fpm
 
LABEL maintainer="PHCM"

RUN docker-php-ext-install pdo_mysql
RUN pecl install xdebug \
    && docker-php-ext-enable xdebug
COPY --from=composer:latest /usr/bin/composer /usr/local/bin/composer
