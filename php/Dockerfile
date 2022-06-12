FROM php:8.1-fpm-alpine

# RUN apk add --update --no-cache --virtual .ext-deps \
#   imagemagick \
#   pcre-dev \
#   icu-dev

# RUN \
#   docker-php-ext-configure opcache 
# RUN \
#   docker-php-ext-install opcache
# RUN \
#   docker-php-ext-install mysqli 

# RUN \
#   # pecl install redis && \
#   pecl install mongodb && \
#   pecl clear-cache

# RUN \
#   docker-php-ext-enable mongodb && \
#   docker-php-source delete

ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS="0" \
    PHP_OPCACHE_MAX_ACCELERATED_FILES="10000" \
    PHP_OPCACHE_MEMORY_CONSUMPTION="192" \
    PHP_OPCACHE_MAX_WASTED_PERCENTAGE="10"

RUN docker-php-ext-install opcache

COPY ./php/opcache.ini /usr/local/etc/php/conf.d/opcache.ini

COPY ./src /app
