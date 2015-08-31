# mojo/Dockerfile

FROM cthulhuology/java

# Install dependencies needed to run ISE
#RUN apt-get install -y libx11-6 libglib2.0-0 libsm6 libxi6 libxrender1 libxrandr2 libfreetype6 libfontconfig1 libxcursor1 libxext6 libxtst6

# Install AVRdude
RUN apt-get install -y avrdude

# Install Mojo tools loaded 1.2.1 and ide 1.1.9
RUN wget https://embeddedmicro.com/media/wysiwyg/mojo-loader/mojo-loader-1.2.1-linux64.tgz
RUN wget https://embeddedmicro.com/ide/mojo-ide-B1.1.9-linux64.tgz
RUN cd /opt && tar zxvf /mojo-loader-1.2.1-linux64.tgz
RUN cd /opt && tar zxvf /mojo-ide-B1.1.9-linux64.tgz
RUN rm /mojo-loader-1.2.1-linux64.tgz /mojo-ide-B1.1.9-linux64.tgz

# We'll mount the ISE webpack in /opt/xilinx
RUN mkdir /opt/xilinx

# Lastly we'll run a shell prompt
CMD /bin/bash

