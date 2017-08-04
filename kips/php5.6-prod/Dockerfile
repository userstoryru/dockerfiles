FROM docker-registry:5000/php:5.6-apache

# update
RUN apt-get update

# mysql
RUN apt-get install -y mysql-client

# unoconv
RUN apt-get install -y unoconv sudo

# netcat
RUN apt-get install -y netcat

# mc
RUN apt-get install -y mc
ENV TERM=xterm

# cron
RUN apt-get install -y cron

# clear cron jobs
RUN rm -rf /etc/cron.d/* && rm -rf /etc/cron.daily/* \
    && rm -rf /etc/cron.hourly/* && rm -rf /etc/cron.monthly/* && rm -rf /etc/cron.weekly/*

WORKDIR /data
