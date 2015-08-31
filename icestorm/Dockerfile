# icestorm/Dockerfile
#
# © 2015 David J Goehrig
#

FROM cthulhuology/
MAINTAINER Dave Goehrig <dave@dloh.org>
RUN apt-get install -y gawk tcl pkg-config clang

# install ftdi dev tools
RUN apt-get install -y libftdi-dev

# install the icestorm components from git
RUN git clone https://github.com/cliffordwolf/icestorm.git icestorm
RUN cd icestorm && make -j$(nproc)
RUN cd icestorm && make install

# install arachne-pnr
RUN git clone https://github.com/cseed/arachne-pnr.git arachne-pnr
RUN cd arachne-pnr && make -j$(nproc)
RUN cd arachne-pnr && make install

# install yosys
RUN git clone https://github.com/cliffordwolf/yosys.git yosys
RUN cd yosys && make -j$(nproc)
RUN cd yosys && make install
