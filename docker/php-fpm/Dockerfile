FROM php:8.3-fpm

RUN apt update -y && apt upgrade -y

COPY --from=mlocati/php-extension-installer /usr/bin/install-php-extensions /usr/local/bin/

RUN install-php-extensions xdebug redis pdo_mysql
