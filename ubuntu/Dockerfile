# ubuntu/Dockerfile
# 
# © 2015 David J Goehrig
#

FROM ubuntu:14.04
MAINTAINER Dave Goehrig <dave@dloh.org>

# upgrade the base image
#
#	* shutup dpkg console bits
# 	* enable mutliverse
# 	* update
#	* upgrade

ENV DEBIAN_FRONTEND=noninteractive
RUN sed -i 's/# \(.*multiverse$\)/\1/g' /etc/apt/sources.list
RUN apt-get update
RUN apt-get -y upgrade

# install build tools and fundamentals

RUN apt-get install -y build-essential
RUN apt-get install -y software-properties-common
RUN apt-get install -y curl git man unzip vim wget python

# Finally we want a shell prompt

CMD /bin/bash


