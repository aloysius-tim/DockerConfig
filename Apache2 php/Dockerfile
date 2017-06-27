FROM eboraas/apache-php

RUN apt-get update

RUN apt-get install software-properties-common -y --fix-missing
RUN apt-add-repository ppa:ondrej/php
RUN apt-get update

#RUN apt-get -y purge php5 libapache2-mod-php5 php5 php5-cli php5-common php5-curl php5-gd php5-imap php5-intl php5-json php5-mcrypt php5-mysql php5-pspell php5-readline php5-sqlite -y

#RUN apt-get install php

RUN apt-get install -y curl --fix-missing
RUN apt-get install -y git --fix-missing
RUN apt-get install -y nano --fix-missing
RUN apt-get install -y php-curl --fix-missing --allow-unauthenticated

RUN a2dismod php5*
#RUN a2enmod php7*
RUN a2enmod rewrite


RUN apt-get install composer
RUN npm install -g yarn

RUN service apache2 restart
