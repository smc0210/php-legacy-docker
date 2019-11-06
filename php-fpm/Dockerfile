FROM php:5.6-fpm-alpine
LABEL wiz <wiz@siot.do>

RUN apk update && \
    # for composer
    apk add zip git && \
    apk add --no-cache \
    # for intl
    icu-dev \
    # for zip
    zlib-dev libzip-dev && \
    docker-php-ext-install opcache intl bcmath zip pdo_mysql

RUN  rm -rf /var/cache/apk/*

COPY ./opcache.ini /usr/local/etc/php/conf.d/opcache.ini

WORKDIR /var/www

CMD ["php-fpm"]

EXPOSE 9000