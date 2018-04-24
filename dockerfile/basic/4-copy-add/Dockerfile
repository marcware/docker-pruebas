FROM ubuntu
RUN apt-get update
RUN apt-get install -y php

##WORKDIR
RUN mkdir /datos
#Este es el direcotrio de trabajo actual
WORKDIR /datos
RUN touch docker.txt

##COPY
#punto hace recerencia al último workdir
#copiamos los ficheros al contenedor
COPY index.php .
COPY app.log /datos

CMD ["/bin/bash"]