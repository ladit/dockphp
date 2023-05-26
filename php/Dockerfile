ARG PHP_VERSION=8

FROM php:${PHP_VERSION}-fpm

ARG PHP_EXTENSIONS="bcmath gd grpc mcrypt mongodb opcache pdo_mysql protobuf rdkafka redis xdebug xlswriter yaml"

ADD https://github.com/mlocati/docker-php-extension-installer/releases/latest/download/install-php-extensions /usr/local/bin/

RUN set -eux; \
  chmod +x /usr/local/bin/install-php-extensions; \
  install-php-extensions ${PHP_EXTENSIONS}

WORKDIR /var/www
