FROM daocloud.io/library/php:7.3

COPY config/php.ini /usr/local/etc/php

#RUN apk add autoconf gcc \
#    && wget https://github.com/phpredis/phpredis/archive/3.1.3.tar.gz \
#    && tar -zxvf 3.1.3.tar.gz \
#    && cd phpredis-3.1.3 \
#    && /usr/local/bin/phpize \
#    && ./configure --with-php-config=/usr/local/bin/php-config \
#    && make \
#    && make install \

ENV PHPREDIS_VERSION 5.0.2
ENV SWOOLE_VERSION 4.4.2

RUN cd ~ \
    && docker-php-ext-install pdo_mysql mysqli pcntl gd\

    && curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/bin/ --filename=composer \
