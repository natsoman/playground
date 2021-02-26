FROM php:7.4.3-fpm

RUN apt-get update && apt-get install -y \
    && librdkafka-dev

# kafka ext
RUN pecl install rdkafka \
    && docker-php-ext-enable rdkafka

# redis ext
RUN pecl install redis \
    && docker-php-ext-enable redis

# xdebug ext
RUN pecl install xdebug \
    && docker-php-ext-enable xdebug \
    && echo "xdebug.mode=debug" >> /usr/local/etc/php/conf.d/docker-php-ext-xdebug.ini

# composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

WORKDIR /var/www

EXPOSE 9000