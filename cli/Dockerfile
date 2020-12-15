FROM wordpress:cli-php7.4

USER root
RUN apk add --no-cache --virtual .build-deps libxml2-dev && docker-php-ext-install soap && apk del .build-deps && apk add --virtual .wordpress-phpexts-rundeps libxml2

USER www-data
