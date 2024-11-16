FROM php:8.3-fpm

RUN pecl install xdebug

RUN  docker-php-ext-install mysqli pdo pdo_mysql \
    && docker-php-ext-enable pdo_mysql xdebug

COPY ./docker/php/custom-php.ini /usr/local/etc/php/conf.d/99-custom-php.ini
