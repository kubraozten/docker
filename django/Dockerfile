FROM ubuntu:latest

MAINTAINER Kubra OZTEN

RUN apt-get update

RUN apt-get install python3-pip python3-dev

RUN pip3 install virtualenv

EXPOSE 8000

ENTRYPOINT ["django"]
CMD ["-g", "daemon off;"]