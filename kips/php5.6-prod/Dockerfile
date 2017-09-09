FROM userstoryru/php5.6-apache

# update
RUN apt-get update

# mysql
RUN apt-get install -y mysql-client

# unoconv
RUN apt-get install -y unoconv sudo

# mc
RUN apt-get install -y mc
ENV TERM=xterm

WORKDIR /data
