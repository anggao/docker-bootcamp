FROM ubuntu:14.04
MAINTAINER Ang Gao

RUN apt-get update && apt-get install -y wget build-essential python python-dev python-pip

RUN wget http://nodejs.org/dist/node-latest.tar.gz && tar xzvf node-latest.tar.gz && cd node-v*

WORKDIR /data

EXPOSE 80
