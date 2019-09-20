FROM php:7.2-fpm

# 安装redis和pdo_mysql扩展
RUN pecl install redis-4.0.1 \
    && docker-php-ext-enable redis \
    && docker-php-ext-install pdo_mysql

# 安装composer
RUN php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');" && \
	php composer-setup.php && \
	php -r "unlink('composer-setup.php');" && \
	mv composer.phar /usr/local/bin/composer && \
	composer self-update