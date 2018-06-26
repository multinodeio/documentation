# rancheros-config

# Install cmd
sudo ros install -c cloud-config.yml -d /dev/nvme0d1 -p /dev/nvme0d1p1

# Format HDD
sudo /sbin/mkfs.ext4 /dev/sda

# Serial Number
sudo apt install dmidecode

sudo /usr/sbin/dmidecode -s system-serial-number

# Docker Volumes

docker volume create geth

# Templates Docs 

http://portainer.readthedocs.io/en/latest/templates.html#stack-template-definition-format

# docker-compose.yml

This file in the 'files' repo has the definitions for the different cloud-config.yml / docker-compose entries and a long ass command line option.

# Stack

RancherOS -> Docker -> Portainer -> templates.json -> multinode/app/dockerfile -> done!