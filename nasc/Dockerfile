# nasc/Dockerfile
#
# © 2015 David J. Goehrig <dave@dloh.org>
#

FROM cthulhuology/x11
MAINTAINER Dave Goehrig <dave@dloh.org>

# Install X11 client & server
RUN add-apt-repository ppa:gnome3-team/gnome3-staging
RUN add-apt-repository ppa:gnome3-team/gnome3
RUN apt-add-repository ppa:nasc-team/daily
RUN apt-get update
RUN apt-get install -y nasc 

# Let the command be a shell script

CMD /bin/bash
