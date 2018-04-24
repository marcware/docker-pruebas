FROM ubuntu
RUN apt-get update
RUN apt-get install -y php

##EXPOSE
RUN apt-get install -y apache2
EXPOSE 80

RUN mkdir /datos
WORKDIR /datos
ADD entrypoint.sh /datos
#sudo chmod +x entrypoint.sh (Pero en el documento local!)
CMD /datos/entrypoint.sh

