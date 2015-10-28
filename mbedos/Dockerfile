# mbedos/Dockerfile
# 
# © 2015 David J Goehrig
#

FROM cthulhuology/ubuntu
MAINTAINER Dave Goehrig <dave@dloh.org>

RUN apt-get update 
RUN apt-get install -y python-setuptools cmake build-essential ninja-build python-dev libffi-dev libssl-dev 
RUN easy_install pip
RUN pip install yotta
RUN apt-get remove binutils-arm-none-eabi gcc-arm-none-eabi
RUN add-apt-repository ppa:terry.guo/gcc-arm-embedded
RUN apt-get update
RUN apt-get install gcc-arm-none-eabi

RUN echo 'eval "$(register-python-argcomplete yotta)"' >> ~/.bashrc
RUN echo 'eval "$(register-python-argcomplete yt)"' >> ~/.bashrc

CMD /bin/bash
