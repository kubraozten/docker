FROM ubuntu:latest

MAINTAINER Kubra OZTEN

RUN apt-get update

RUN apt-get install -y nginx

RUN curl -o /etc/nginx/sites-available/django21 https://github.com/kubraozten/nginx/django21

RUN ln -s /etc/nginx/sites-available/django21 /etc/nginx/sites-enabled

RUN rm -rf sites-enabled/default

RUN service nginx restart

EXPOSE 80

ENTRYPOINT nginx -g 'daemon off;'