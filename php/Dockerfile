FROM php:8-fpm-alpine

RUN set -eux; \
  apk add --no-cache tzdata $PHPIZE_DEPS libmcrypt-dev yaml-dev librdkafka-dev; \
  cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime; \
  pecl channel-update pecl.php.net; \
  pecl install mcrypt xdebug redis rdkafka mongodb yaml xlswriter; \
  docker-php-ext-install opcache pdo_mysql bcmath; \
  docker-php-ext-enable xdebug redis rdkafka mongodb yaml xlswriter; \
  apk del tzdata $PHPIZE_DEPS;

WORKDIR /var/www
