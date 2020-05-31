# rpi-ansible
Raspberry Pi 4 Ansible playbooks with Hassio in Docker, Portainer, and RetroPie


## Install Ansible on your machine

brew install ansible

## Add hosts config

Edit and copy hosts file to the /etc/ansible/hosts

## Copy your public SSH key to the RPi

ssh-copy-id -i ~/.ssh/id_rsa.pub user@host

## Check Raspberry availability for Ansible

ansible all -m ping -u pi

## Run playbook

ansible-playbook -u pi deploy.yaml