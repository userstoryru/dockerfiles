FROM debian:jessie

# update
RUN apt-get update

# install php
RUN apt-get install -y \
    php5-cli \
    php5-common \
    php5-curl \
    php5-gd \
    php5-imagick \
    php5-intl \
    php5-json \
    php5-ldap \
    php5-mcrypt \
    php5-memcache \
    php5-memcached \
    php5-mhash \
    php5-mongo \
    php5-mysql \
    php5-pgsql \
    php5-readline \
    php5-redis \
    php5-sqlite \
    php5-dev \
    php-pear

# install deps
RUN apt-get -y install pkg-config

# install mongo
RUN pecl install mongodb && echo "extension=mongodb.so" > /etc/php5/cli/conf.d/20-mongo.ini 

# configure php
RUN echo "date.timezone = UTC" >> /etc/php5/cli/php.ini
