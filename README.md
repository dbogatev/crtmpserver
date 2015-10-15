HowTo build and install crtmpserver

Requirements:
* GCC and other C++ tools
* SVN
* libdl, libssl, libcrypto

#Setup Requirements

apt-get install build-essential libssl-dev cmake

#Compile and Install:

cd crtmpserver/builders/cmake
cmake -DCRTMPSERVER_INSTALL_PREFIX=/opt/crtmpserver
make
make install

#If you preffer to create debian package

apt-get install dh-make
cd crtmpserver/builders/packing/debian
bash build_package.sh

