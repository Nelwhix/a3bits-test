FROM php:7.4-fpm-alpine

RUN docker-php-ext-install pdo pdo_mysql

RUN apk --update add --virtual build-dependencies build-base openssl-dev autoconf \
  && pecl install pecl_http-3.3.0 \
  && docker-php-ext-enable pecl_http \
  && apk del build-dependencies build-base openssl-dev autoconf \
  && rm -rf /var/cache/apk/*