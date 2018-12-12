BootStrap: debootstrap
OSVersion: xenial
MirrorURL: http://us.archive.ubuntu.com/ubuntu/

%post
 
    echo "deb http://nova.clouds.archive.ubuntu.com/ubuntu/ xenial-backports main restricted universe multiverse" | tee -a /etc/apt/sources.list
    echo "deb http://nova.clouds.archive.ubuntu.com/ubuntu/ xenial main restricted" | tee -a /etc/apt/sources.list
    echo "deb http://nova.clouds.archive.ubuntu.com/ubuntu/ xenial multiverse" | tee -a /etc/apt/sources.list
    echo "deb http://nova.clouds.archive.ubuntu.com/ubuntu/ xenial universe" | tee -a /etc/apt/sources.list
    echo "deb http://nova.clouds.archive.ubuntu.com/ubuntu/ xenial-updates main restricted" | tee -a /etc/apt/sources.list
    echo "deb http://nova.clouds.archive.ubuntu.com/ubuntu/ xenial-updates multiverse" | tee -a /etc/apt/sources.list
    echo "deb http://nova.clouds.archive.ubuntu.com/ubuntu/ xenial-updates universe" | tee -a /etc/apt/sources.list
    echo "deb http://security.ubuntu.com/ubuntu xenial-security main restricted" | tee -a /etc/apt/sources.list
    echo "deb http://security.ubuntu.com/ubuntu xenial-security multiverse" | tee -a /etc/apt/sources.list
    echo "deb http://security.ubuntu.com/ubuntu xenial-security universe" | tee -a /etc/apt/sources.list
    echo "deb-src http://nova.clouds.archive.ubuntu.com/ubuntu/ xenial-backports main restricted universe multiverse" | tee -a /etc/apt/sources.list
    echo "deb-src http://nova.clouds.archive.ubuntu.com/ubuntu/ xenial main restricted" | tee -a /etc/apt/sources.list
    echo "deb-src http://nova.clouds.archive.ubuntu.com/ubuntu/ xenial multiverse" | tee -a /etc/apt/sources.list
    echo "deb-src http://nova.clouds.archive.ubuntu.com/ubuntu/ xenial universe" | tee -a /etc/apt/sources.list
    echo "deb-src http://nova.clouds.archive.ubuntu.com/ubuntu/ xenial-updates main restricted" | tee -a /etc/apt/sources.list
    echo "deb-src http://nova.clouds.archive.ubuntu.com/ubuntu/ xenial-updates multiverse" | tee -a /etc/apt/sources.list
    echo "deb-src http://nova.clouds.archive.ubuntu.com/ubuntu/ xenial-updates universe" | tee -a /etc/apt/sources.list
    echo "deb-src http://security.ubuntu.com/ubuntu xenial-security main restricted" | tee -a /etc/apt/sources.list
    echo "deb-src http://security.ubuntu.com/ubuntu xenial-security multiverse" | tee -a /etc/apt/sources.list
    echo "deb-src http://security.ubuntu.com/ubuntu xenial-security universe" | tee -a /etc/apt/sources.list
 
    apt-get -y update
    apt-get -y upgrade
    apt-get install -y curl wget tar gzip gcc build-essential zlib1g-dev
    wget -O bsmap-2.90.tgz http://lilab.research.bcm.edu/dldcc-web/lilab/yxi/bsmap/bsmap-2.90.tgz
    mkdir software
    tar -xvzf bsmap-2.90.tgz
    cp -R bsmap-2.90/ software/bsmap-2.90
    cd software/bsmap-2.90
    make
    make install
     
% environment 
  export PATH=/software/bsmap-2.90:$PATH
 
