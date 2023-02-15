
# What is  My Lab
> My lab is to experiment and learn—critical tasks for pursuing cloud computing, Linux, learning new automation tools for setting up the cloud environment, improving DevOps work skills, or experimenting with cloud services.

![Tools on WSL](wsl.PNG)

| Name | Description | Updated Date |
| ----------- | ----------- | ----------- |
| Blog | GitHub Blog Site [Read more...](https://dial2vincent.github.io/) | 2023 |
| Lab | Markdown Samples [Read more...](https://github.com/dial2vincent/lab) | Today |
--- 
## Build your lab environment 
- Host Operating System: Linux, Windows, Mac
- Virtual Machines: AWS, Hyper-V, VirtualBox
  - Guest operating systems: RHEL, CentOS Streams, Oracle Linux, Ubuntu, Windows server

## Laptop
### WSL Windows
The Windows Subsystem for Linux lets developers run a GNU/Linux environment -- including most command-line tools, utilities, and applications -- directly on Windows, unmodified, without the overhead of a traditional virtual machine or dual boot setup.
- How to set up WSL on your labtop  [Read more...](https://github.com/dial2vincent/wsl)
- What applications and packages are installed on the WSL?
- [x] Application Installed on WSL: Ansible, Code, Docker, Packer, Python, Python3, Terraform
- [x] Package Installed on WSL: Bash
- [x] Application Installed on Windows: Vagrant, Virtualbox 
- [ ] Need to be Installed: Java, Jenkins, Kubernetes

## Virtual Machines 
### AWS [^1]
1. Master node: myvm, Utility Server (myvm) Requirement Tools: 
- [x] Application installed on AWS: Ansible, Docker, Git, Jenkins, Packer, Terraform
- [x] Package installed on AWS: Bash, Java, Maven, Python, Python3
- [x] Need to be installed: Visual Studio Code, Kubernetes
2. Managed node: myweb, Web Server (myweb) Requirement Tools: 
- [x] Application installed on AWS: Packer, Git, Tomcat
- [x] Package installed on AWS: Java, Python, Python3, Maven, Bash
- [ ] Need to Installed:
 
### Hyper-V [^2]
- Kubernetes master node: oracle
  - Worker Nodes: oracle1, oracle2 
- Ansible control node: utility
  - Managed node: oracle1, oracle2, ubunt2 

### VirtualBox [^3]
B:
- Kubernetes master node: K8s
  - Worker Nodes: k8s-n1, k8s-n2 
- Ansible control node: ansible
  - Managed Node: n/a 
- something here 
 
 ### Guinea
 - red
 - kitchen
 - master
 - office
 
[^1]: Location: AWS, Hosts: myvm, myweb 
[^2]: Location: Windows 2012 Hyper-v
[^3]: Location: B

## Tracking the CHANGELOG.md
1. Ansible Host Nodes: node1, ~~node2~~
2. Web Server: myweb, Requirement Tools: Tomcat server,
  
## Tips & Notes
### How to find your Github Repo Size
- Opening your Account Settings → Repositories (https://github.com/settings/repositories), and the repository size is displayed next to its designation.
