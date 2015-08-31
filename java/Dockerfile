# java/Dockerfile
#
# © 2015 David J. Goehrig <dave@dloh.org>
#

FROM cthulhuology/x11
MAINTAINER Dave Goehrig <dave@dloh.org>

# Install Oracle Java8 
#
#	* use the accept license trick
#	* install via ppa
#	* cleanup

RUN echo oracle-java8-installer shared/accepted-oracle-license-v1-1 select true | debconf-set-selections
RUN add-apt-repository -y ppa:webupd8team/java
RUN apt-get update
RUN apt-get install -y oracle-java8-installer
RUN rm -rf /var/lib/apt/lists/*
RUN rm -rf /var/cache/oracle-jdk8-installer

# Set Java envars

ENV JAVA_HOME /usr/lib/jvm/java-8-oracle

# Let the command be a shell script

CMD /bin/bash
