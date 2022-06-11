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

COPY ./src /app