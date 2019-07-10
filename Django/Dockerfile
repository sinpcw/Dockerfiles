FROM ubuntu:18.04
MAINTAINER sinpcw

# Command
CMD ["echo", "Simple Django Project"]

RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install -y vim-common && \
    apt-get install -y curl python3 python3-pip && \
    pip3 install django
