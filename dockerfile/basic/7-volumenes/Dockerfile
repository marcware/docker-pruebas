FROM ubuntu
RUN apt-get update
RUN apt-get install -y zip unzip
RUN apt-get install -y php \
    php-cli

RUN apt-get install -y apache2 \
    libapache2-mod-php
EXPOSE 80

RUN mkdir /datos
WORKDIR /datos
ADD entrypoint.sh /datos

##VOLUME
ADD paginas /var/www/html
VOLUME ["/var/www/html"]

#sudo chmod +x entrypoint.sh (Pero en el documento local!)
CMD /datos/entrypoint.sh

