FROM nimmis/apache-php7

RUN apt-get update

RUN apt-get install -y curl --fix-missing
RUN apt-get install -y git --fix-missing
RUN apt-get install -y nano --fix-missing
RUN apt-get install -y php-curl --fix-missing --allow-unauthenticated

RUN a2enmod rewrite

RUN apt-get install composer

RUN service apache2 restart
