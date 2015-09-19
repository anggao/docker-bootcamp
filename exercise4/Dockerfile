FROM ubuntu:14.04
MAINTAINER Ang Gao

RUN apt-get update
ADD hello.sh /
RUN chmod +x /hello.sh

ENTRYPOINT /hello.sh
