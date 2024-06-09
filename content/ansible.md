# Ansible
## Ansible Installation
`sudo yum install ansible`\
`ansible --version`\
` ansible -m setup localhost | grep ansible_python_version`
## Ansible Inventory
- Add inventory on /etc/ansible/hosts
- Display inventory hosts \
`ansible all --list-hosts`\
`ansible oracle_linux  --list-hosts`
