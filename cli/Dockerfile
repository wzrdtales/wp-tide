FROM wordpress:cli-php7.4

USER root
RUN apk add --no-cache --virtual .wordpress-phpexts-rundeps libxml2 && docker-php-ext-install soap 

USER www-data
