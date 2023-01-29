
# What is  mylab
> The mylab is to experiment and learn—critical tasks for pursuing cloud computing, Linux, learning a new automation tools for setting up the cloud environment, improving devops work skills, or experimenting with cloud services.

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
### AWS 
1. Master node: myvm 
Utility Server (myvm) Requirement Tools: 
- [x] Application Installed on AWS: Ansible, Code, Docker, Packer, Shell, Terraform
- [x] Package Installed on AWS: Python, Python3, Maven, Shell, Bash
- [x] Application Installed on AWS Linux: 
- [ ] Need to Installed: Java, JDK, Jenkins, Kubernetes
2. Managed node: myweb 
Web Server (myweb) Requirement Tools: 
- [x] Application Installed on AWS: Ansible, Code, Docker, Packer, Shell, Terraform
- [x] Package Installed on AWS: Python, Python3, Maven, Shell, Bash
- [x] Application Installed on AWS Linux: Tomcat
- [ ] Need to Installed: Java, JDK, Jenkins, Kubernetes

### Hyper-V
- Kubernetes master node: K8s
  - Worker Nodes: k8s-node1, k8s-node2 [^1]
- Ansible control node: utility
  - Managed node: node1, node2 [^2]

### VirtualBox
- Kubernetes master node: K8s
  - Worker Nodes: k8s-node1, k8s-node2 [^1]
- Ansible control node: utility
  - Managed node: node1, node2 [^2]
- something here [^3]
 
[^1]: Location: hyper-v
[^2]: Location: aws
[^3]: Location: aws

## Tracking the CHANGELOG.md
~~The node2 host is flat.~~
1. Ansible Host Nodes: node1, node2
2. Web Server: myweb
  - Requirement Tools: Tomcat server,
  
## Tips & Notes
### How to find your Github Repo Size
- Opening your Account Settings → Repositories (https://github.com/settings/repositories), and the repository size is displayed next to its designation.
