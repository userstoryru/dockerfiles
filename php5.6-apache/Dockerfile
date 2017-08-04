FROM userstoryru/php5.6

# update
RUN apt-get update

# install apache
RUN apt-get install -y apache2 libapache2-mod-rpaf libapache2-mod-php5 \
    && a2enmod rewrite \
    && a2enmod rpaf \
    && a2enmod proxy \
    && a2enmod proxy_http

# configure php
RUN echo "date.timezone = UTC" >> /etc/php5/apache2/php.ini

COPY apache2-foreground /usr/bin/
WORKDIR /data

EXPOSE 80
CMD ["apache2-foreground"]
