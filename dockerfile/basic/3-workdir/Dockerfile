FROM ubuntu
RUN apt-get update
RUN apt-get install -y php
RUN mkdir /datos
#Este es el direcotrio de trabajo actual
WORKDIR /datos
RUN touch docker.txt
CMD ["/bin/bash"]