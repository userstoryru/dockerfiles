FROM userstoryru/php:5.6-apache

# update
RUN apt-get update

# mysql
RUN apt-get install -y mysql-client

# unoconv
RUN apt-get install -y unoconv sudo

# unoconv hack
RUN chown -R www-data:www-data /var/www && sudo -u www-data unoconv -f pdf foo >/dev/null 2>&1 || true

# mc
RUN apt-get install -y mc
ENV TERM=xterm

# graphviz
RUN apt-get install -y graphviz

# ffmpeg
RUN echo deb http://ftp.uk.debian.org/debian jessie-backports main >>/etc/apt/sources.list
RUN apt-get update
RUN apt-get install -y ffmpeg

WORKDIR /data
