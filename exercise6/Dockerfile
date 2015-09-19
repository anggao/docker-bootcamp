FROM ubuntu:14.04
MAINTAINER Ang Gao

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update
RUN apt-get -y install apache2

ENV APACHE_RUN_USER www-data
ENV APACHE_RUN_GROUP www-data
ENV APACHE_PID_FILE /var/run/apache2.pid
ENV APACHE_RUN_DIR /var/run/apache2

RUN mkdir /var/lock/apache2

ENV APACHE_LOCK_DIR /var/lock/apache2
ENV APACHE_LOG_DIR /var/log/apache2

ADD index.html /var/www/html/

EXPOSE 80

CMD ["apache2", "-D", "FOREGROUND"]
