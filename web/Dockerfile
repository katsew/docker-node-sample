FROM nginx:1.9.6
MAINTAINER mlkato

RUN apt-get -y update
RUN apt-get -y install vim
RUN rm /etc/nginx/conf.d/default.conf

ADD app.conf /etc/nginx/conf.d/app.conf
