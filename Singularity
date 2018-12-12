BootStrap: debootstrap
OSVersion: xenial
MirrorURL: http://us.archive.ubuntu.com/ubuntu/
 
%files
    someLocalFile /opt/
 
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
 
    # make sure everything is uptodate
#    apt-get -y --allow-unauthenticated update
#    apt-get -y --allow-unauthenticated upgrade
 
    mkdir <relative path>
    wget -O <relative path>/<thing to download.zip> http://URL
