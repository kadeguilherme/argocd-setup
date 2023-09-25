FROM ubuntu:latest
LABEL name="Guilherme Aguiar"
LABEL email="kadeguilherme@gmail.com"
RUN apt-get update -y
ENV DEBIAN_FRONTEND noninteractive	
RUN apt-get -y install tzdata
RUN apt-get install apache2 -y
WORKDIR /var/www/html/
COPY /script/index.html /var/www/html/
EXPOSE 80
CMD ["apachectl" , "-D","FOREGROUND"]