############################################################
# Dockerfile to build base container images
# Based on official ubuntu image
############################################################
# Set the base image to official ubuntu
FROM ubuntu
# File Author / Maintainer
MAINTAINER sgyzetrov
################## BEGIN INSTALLATION ######################
RUN cp /etc/apt/sources.list /etc/apt/sources.list.bak &&\
echo "# 163\ndeb http://mirrors.163.com/ubuntu/ bionic main restricted universe multiverse\ndeb http://mirrors.163.com/ubuntu/ bionic-security main restricted universe multiverse\ndeb http://mirrors.163.com/ubuntu/ bionic-updates main restricted universe multiverse\ndeb http://mirrors.163.com/ubuntu/ bionic-proposed main restricted universe multiverse\ndeb http://mirrors.163.com/ubuntu/ bionic-backports main restricted universe multiverse\ndeb-src http://mirrors.163.com/ubuntu/ bionic main restricted universe multiverse\ndeb-src http://mirrors.163.com/ubuntu/ bionic-security main restricted universe multiverse\ndeb-src http://mirrors.163.com/ubuntu/ bionic-updates main restricted universe multiverse\ndeb-src http://mirrors.163.com/ubuntu/ bionic-proposed main restricted universe multiverse\ndeb-src http://mirrors.163.com/ubuntu/ bionic-backports main restricted universe multiverse">sources.list &&\
cp -f sources.list /etc/apt/sources.list &&\
echo "==> Installing curl, wget, man-db, inetutils-ping, net-tools, coreutils, bsdmainutils, tree, vim, bzip2, unzip，add-apt-repository, build-essential (gcc, g++, make, dpkg-dev), screenfetch"  && \  
apt-get update               && \
apt-get install -y curl wget man-db inetutils-ping net-tools coreutils bsdmainutils tree vim bzip2 unzip make software-properties-common build-essential screenfetch && \
echo "==> Done for now, enjoy your base image..."
# echo "==> [Deprecated] Add ppa for version of gcc-6..."  && \
# add-apt-repository ppa:ubuntu-toolchain-r/test  && \
# apt-get update               && \
# apt-get install -y gcc-6 g++-6 && \
##################### INSTALLATION END #####################
# TODO
# TBA
