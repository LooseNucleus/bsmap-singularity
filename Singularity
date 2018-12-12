BootStrap: docker 
From: ubuntu:16.04

%post 
mkdir -p /software
apt-get update
apt-get install -y curl wget tar gzip 
wget http://lilab.research.bcm.edu/dldcc-web/lilab/yxi/bsmap/bsmap-2.90.tgz
tar -xvzf bsmap-2.90.tgz 
cp -R bsmap-2.90/ /software/
rm -rf bsmap-2.90


