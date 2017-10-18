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

# ffmpeg
RUN echo deb http://ftp.uk.debian.org/debian jessie-backports main >>/etc/apt/sources.list
RUN apt-get update
RUN apt-get install -y ffmpeg

WORKDIR /data
