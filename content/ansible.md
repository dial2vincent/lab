
# Ansible

## Installation
~~~
sudo yum install ansible -y
ansible --version
~~~
## Configuration
Location: /etc/ansible 
- ansible.cfg
~~~
# Since Ansible 2.12 (core):
# To generate an example config file (a "disabled" one with all default settings, commented out):
#               $ ansible-config init --disabled > ansible.cfg
#
# Also you can now have a more complete file by including existing plugins:
# ansible-config init --disabled -t all > ansible.cfg

# For previous versions of Ansible you can check for examples in the 'stable' branches of each version
# Note that this file was always incomplete  and lagging changes to configuration settings

# for example, for 2.9: https://github.com/ansible/ansible/blob/stable-2.9/examples/ansible.cfg

[default]
inventory = ./hosts
host_key_checking = False
forks             = 20
gathering = explicit
action_warnings= False

[privilege_escalation]
become=True
~~~
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
