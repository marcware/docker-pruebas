En esta contenedor cunado se cree, automáticamente accederá a el bash

#### Creamos la imagen, que tiene el dockerfile en local
$ docker build -t imagen_php:v1 .

#### Vemos el histori de la imagen
$ docker image history imagen_php:v1

#### Creamos el contenedor
$ docker run -it --rm imagen_php:v1

#### EXPOSE
$ docker run -it --rm -p 8080:80 imagen_php:expose

#### VOLUME
#Carpeta de volumes cd /var/lib/docker/volumes/
$ docker volume ls
$ docker run -it --rm -p 8080:80 --name c1 imagen_php:volume 
#Pilla el volumen de c1
$ docker run -it --rm -p 9080:80 --volumes-from c1 --name c2 imagen_php:volume
