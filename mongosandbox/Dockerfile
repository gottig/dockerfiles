# Docker file to build mongoDB
#############################

# Set the base image to Ubuntu
FROM ubuntu

MAINTAINER Avinash

################## BEGIN INSTALLATION ##################
# Add package verification key
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 7F0CEB10


RUN echo 'deb http://downloads-distro.mongodb.org/repo/ubuntu-upstart dist 10gen' | tee /etc/apt/sources.list.d/mongodb.list

RUN apt-get update

RUN apt-get install -y mongodb-10gen

RUN mkdir -p /data/db

################## COMPLETE INSTALLATION ##################

EXPOSE 27017

CMD ["--port 27017"]

ENTRYPOINT usr/bin/mongod


