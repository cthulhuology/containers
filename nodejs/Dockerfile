# ubuntu/Dockerfile
# 
# © 2015 David J Goehrig
#

FROM cthulhuology/ubuntu
MAINTAINER Dave Goehrig <dave@dloh.org>

RUN curl -O https://nodejs.org/dist/v0.12.7/node-v0.12.7-linux-x64.tar.gz
RUN tar -C /usr/local --strip-components=1 -zxvf /node-v0.12.7-linux-x64.tar.gz 
RUN rm /node-v0.12.7-linux-x64.tar.gz

CMD /bin/bash


