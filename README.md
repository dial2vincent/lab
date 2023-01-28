
# What is cloud lab
> Create your Lab to experiment and learn—critical tasks for pursuing cloud computing, Linux, learning a new automation tools for setting up the cloud environment, devops work skills, or experimenting with services.

![Tools on WSL](wsl.PNG)

| Name | Description | Updated Date |
| ----------- | ----------- | ----------- |
| blog | [Read more...](https://dial2vincent.github.io/) | 2023 |
| lab | Markdown Samples [Read more...](https://github.com/dial2vincent/lab) | Today |
--- 
## Build your lab environment 
- Host Operating System: Linux, Windows, Mac
- Virtual Machines: AWS, Hyper-V, VirtualBox
- Guest operating systems: RHEL, CentOS Streams, Oracle Linux, Ubuntu, Windows server

## Laptop
### WSL Windows
The Windows Subsystem for Linux lets developers run a GNU/Linux environment -- including most command-line tools, utilities, and applications -- directly on Windows, unmodified, without the overhead of a traditional virtual machine or dualboot setup.
- How to set up WSL on your labtop  [Read more...](https://github.com/dial2vincent/wsl)
- Ansible, Python, Python3, Bash, Code, Docker, Jenkins, Java, JDK, Kubernetes, Maven, Packer, Shell, Terraform, Vagrant, Virtualbox, 
- [x] Application Installed on WSL: Ansible, Code, Docker, Packer, Terraform
- [x] Package Installed on WSL: Python, Python3, Maven, Shell, Bash
- [x] Application Installed on Windows: Vagrant, Virtualbox 
- [ ] Need to Installed: Java, JDK, Jenkins, Kubernetes

## Virtual Machines 
### AWS Utility Server Requirement Tools: 

- Ansible, Python, Python3, Bash, Code, Docker, Jenkins, Java, JDK, Kubernetes, Maven, Packer, Shell, Terraform, Vagrant, Virtualbox, 
- [x] Application Installed on WSL: Ansible, Code, Docker, Packer, Shell, Terraform
- [x] Package Installed on WSL: Python, Python3, Maven, Shell, Bash
- [x] Application Installed on Windows: Vagrant, Virtualbox, 
- [ ] Need to Installed: Java, JDK, Jenkins, Kubernetes

### Hyper-V
- Kubernetes Control Node: K8s, Work Nodes: k8s-node1, k8s-node2 [^1]
- Ansible control node: utility, managed node: node1, node2 [^2]
### VirtualBox
- something here [^3]
## Hosts and Guest Operating Systems
Master node: myvm 
Managed node: myweb 

[^1]: Location: hyper-v
[^2]: Location: aws
[^3]: Location: aws

## Hosts and Guest Operating Systems
~~The node2 host is flat.~~
- Ansible Host Nodes: node1, node2

- Web Server: myweb
  - Requirement Tools: Tomcat server,
  
## How to find your Github Repo Size
- Opening your Account Settings → Repositories (https://github.com/settings/repositories), and the repository size is displayed next to its designation.
