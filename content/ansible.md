
# Ansible

## Installation
~~~
sudo yum install ansible -y
ansible --version
~~~
## Configuration
Location: /etc/ansible 
- ansible.cfg
- hosts
inventory\
`ansible-inventory --list`\
`ansible all --list-hosts`\
`ansible oracle_linux  --list-hosts`
## Tutorial

## Demo

## Use case
- ad-hoc command:\
ansible -m setup localhost | grep ansible_python_version
