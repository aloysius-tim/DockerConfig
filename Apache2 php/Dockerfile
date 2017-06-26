FROM eboraas/apache-php

RUN apt-get update

RUN apt-get install software-properties-common -y --fix-missing
RUN apt-add-repository ppa:ondrej/php
RUN apt-get update

RUN apt-get install php7.0 -y
RUN apt-get install libapache2-mod-php7.0 libapache2-mod-php -y

RUN apt-get install -y curl --fix-missing
RUN apt-get install -y git --fix-missing
RUN apt-get install -y nano --fix-missing
RUN apt-get install -y php-curl --fix-missing --allow-unauthenticated

RUN a2dismod php5*
RUN a2enmod php7
RUN a2enmod rewrite


RUN apt-get install composer
RUN npm install -g yarn
RUN npm install -g angular-cli

RUN service apache2 restart
