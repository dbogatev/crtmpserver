crtmpserver
===========

HowTo build and install crtmpserver

Requirements:
* GCC and other C++ tools
* SVN
* libdl, libssl, libcrypto

#Setup Requirements
apt-get install build-essential libssl-dev cmake

#Compile and Install:

cd crtmpserver/builders/cmake
cmake -DCRTMPSERVER_INSTALL_PREFIX=<path> #(for example /opt/crtmpserver)
make
make install

