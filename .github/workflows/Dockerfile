FROM ubuntu:latest
LABEL name="Guilherme Aguiar"
LABEL email="kadeguilherme@gmail.com"
RUN apt-get update -y
ENV DEBIAN_FRONTEND noninteractive	
RUN apt-get -y install tzdata
RUN apt-get install apache2 -y
COPY . /var/www/html/
EXPOSE 80
CMD ["apachectl" , "-D","FOREGROUND"]