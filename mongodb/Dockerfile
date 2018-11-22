FROM ubuntu:latest

MAINTAINER Kubra OZTEN

RUN apt-get update

RUN apt install -y mongodb

EXPOSE 27017

ENTRYPOINT ["mongodb"]
CMD ["-g", "daemon off;"]
