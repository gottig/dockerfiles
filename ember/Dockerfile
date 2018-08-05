FROM node:6.10.0

MAINTAINER Avinash

RUN apt-get update -y && apt-get install --no-install-recommends -y -q \
     vim-tiny

RUN \
     npm install -g ember-cli@2.11 &&\
     npm install -g bower &&\
     npm install -g phantomjs

RUN echo 'alias ll="ls -l"' >> ~/.bashrc

