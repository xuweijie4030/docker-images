FROM php:7.2-fpm

RUN pecl install redis-4.0.1 \
    && docker-php-ext-enable redis \
    && docker-php-ext-install pdo_mysql