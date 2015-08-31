# x11/Dockerfile
#
# © 2015 David J. Goehrig <dave@dloh.org>
#

FROM cthulhuology/ubuntu
MAINTAINER Dave Goehrig <dave@dloh.org>

# Install X11 client & server
RUN apt-get update
RUN apt-get install -y xauth xorg openbox

# Let the command be a shell script

CMD /bin/bash
