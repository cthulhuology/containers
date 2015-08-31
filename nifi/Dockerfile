# nifi/Dockerfile
#
# © 2015 David J. Goehrig <dave@dloh.org>
#

FROM cthulhuology/java
MAINTAINER Dave Goehrig <dave@dloh.org>

# Install nifi
RUN curl -O http://psg.mtu.edu/pub/apache/nifi/0.2.1/nifi-0.2.1-bin.tar.gz
RUN mkdir -p java
RUN cd java && tar zxvf ../nifi-0.2.1-bin.tar.gz

# Ports

EXPOSE 8080


# Let the command be a shell script

CMD /bin/bash
