Docker Containers
-----------------

This repository contains a number of docker containers that I use for playing around with embedded
projects.  Many of these assume you are running an X11 server on your development box.  Some of them
require 3rd party closed source software to be mounted at specific locations to work.  Details on
each can be found in the appropriate places.


Contents
--------

	* ubuntu	-	the base ubuntu 14.04 image used by all of the containers
	* x11		-	an image containing stuff necessary for x11 apps
	* java		- 	Oracle Java 8 JDK on top of x11, used by many 3rd party tools
	* avr		-	AVR tools for programming Arduinos
	* mojo		-	mojo-ide for programming embeddedmicro.com FPGA boards
	* icestorm	-	open source tools for programing the Lattice iCE40HX-1k 
	* synflow	-	Synflow 

