En esta contenedor cunado se cree, automáticamente accederá a el bash

#### Creamos la imagen, que tiene el dockerfile en local
$ docker build -t imagen_php:v1 .

#### Vemos el histori de la imagen
$ docker image history imagen_php:v1

#### Creamos el contenedor
$ docker run -it --rm imagen_php:v1


#### Expose
$ docker run -it --rm -p 8080:80 imagen_php:expose