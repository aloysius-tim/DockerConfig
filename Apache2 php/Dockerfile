FROM eboraas/apache-php

RUN apt-get install software-properties-common

RUN apt-get update
RUN apt-add-repository ppa:ondrej/php
RUN apt-get install -y curl --fix-missing
RUN apt-get install -y git --fix-missing
RUN apt-get install -y nano --fix-missing
RUN apt-get install -y php-curl --fix-missing
RUN apt-get install -y \ php7.0 \php7.0-cli \ php7.0-cgi \ php7.0-fpm \ php7.0-curl \ php7.0-gd \ php7.0-dev \ php7.0-json \ php7.0-mcrypt \ php7.0-mysql \ php7.0-readline \ php7.0-xmlrpc --fix-missing

RUN a2dismod php5*
RUN a2enmod php7*
RUN a2enmod rewrite


RUN apt-get install composer
RUN npm install -g yarn
RUN npm install -g angular-cli

RUN service apache2 restart
