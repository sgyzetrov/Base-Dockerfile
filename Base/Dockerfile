############################################################
# Dockerfile to build base container images
# Based on official ubuntu image
############################################################
# Set the base image to official ubuntu
FROM ubuntu
# File Author / Maintainer
MAINTAINER sgyzetrov
################## BEGIN INSTALLATION ######################
RUN echo "==> Installing curl, wget, man-db, inetutils-ping, net-tools, coreutils, bsdmainutils, tree, vim, bzip2, unzip，add-apt-repository, build-essential (gcc, g++, make, dpkg-dev), screenfetch"  && \  
apt-get update               && \
apt-get install -y curl wget man-db inetutils-ping net-tools coreutils bsdmainutils tree vim bzip2 unzip make software-properties-common build-essential screenfetch && \
echo "==> Done for now, enjoy your base image..."
# echo "==> [Deprecated] Add ppa for version of gcc-6..."  && \
# add-apt-repository ppa:ubuntu-toolchain-r/test  && \
# apt-get update               && \
# apt-get install -y gcc-6 g++-6 && \
##################### INSTALLATION END #####################
# TODO
# Optimize for Chinese ISP