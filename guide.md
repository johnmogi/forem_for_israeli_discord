docker fedora
docker run -it fedora:36 /bin/bash

git
sudo dnf -y update
sudo dnf -y install git
git --version

pip3
sudo dnf install --assumeyes python3-pip
pip3 --version

ansible
sudo dnf -y install https://dl.fedoraproject.org/pub/epel/epel-release-latest-8.noarch.rpm --skip-broken
sudo dnf install  --enablerepo epel-playground ansible 
sudo yum install ansible
ansible --version

butane
https://coreos.github.io/butane/getting-started/

alias butane='podman run --rm --interactive         \
              --security-opt label=disable          \
              --volume "${PWD}":/pwd --workdir /pwd \
              quay.io/coreos/butane:release'


pwgen
sudo dnf makecache --refresh
sudo dnf -y install pwgen

xxd
vim-common 
yum install vim-common 

aws cli