FROM php:7.4-fpm
 
LABEL maintainer="PHCM"

RUN apt-get update && apt-get install -y libmcrypt-dev libonig-dev zlib1g-dev libicu-dev g++ libmagickwand-dev libfreetype6-dev libfontconfig1-dev libpng-dev 
RUN docker-php-ext-configure intl 
RUN docker-php-ext-install pdo_mysql intl gd mbstring
RUN pecl install xdebug imagick mcrypt \
    && docker-php-ext-enable xdebug imagick gd intl mcrypt
COPY --from=composer:latest /usr/bin/composer /usr/local/bin/composer
