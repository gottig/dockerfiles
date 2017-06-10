# Docker file to build mongo university m101p
##########################################################

# Set the base image to Ubuntu
FROM ubuntu:14.04

MAINTAINER Avinash

#ENV MONGO_VERSION 2.6.12
ENV PYTHON_VERSION python2.7

# Installation:
# Import MongoDB public GPG key
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 7F0CEB10

# Create a MongoDB list file
RUN echo 'deb http://downloads-distro.mongodb.org/repo/ubuntu-upstart dist 10gen' | tee /etc/apt/sources.list.d/10gen.list

RUN set -x \
	&& apt-get -y update \
	&& apt-get install -y $PYTHON_VERSION \
	&& apt-get install -y mongodb-org

#	&& apt-get install -y mongodb-org=$MONGO_VERSION

# Expose port mongod 27017
EXPOSE 27017

# Set /usr/bin/mongod as the dockerized entry point
#ENTRYPOINT /usr/bin/mongod
