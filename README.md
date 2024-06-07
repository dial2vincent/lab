
# What is  My Lab
> My lab is to experiment and learn—critical tasks for pursuing cloud computing, Linux, learning new automation tools for setting up the cloud environment, improving DevOps work skills, or experimenting with cloud services.

![Tools on WSL](wsl.PNG)

--- 
## Table of content  
| Name | Type | Description | Link | 
| ----------- | ----------- | ----------- | ----------- |
| Ansible | Configuration push based | xxxx |[more..](https://github.com/dial2vincent/lab) |
| Bash | Linux | |  [more...](https://github.com/dial2vincent/bash) | 
| Docker | Container | | [more..](https://github.com/dial2vincent/lab) |
| Git | Version Control | | [more..](https://github.com/dial2vincent/lab) |
| Github | Git remote repository | |  [more...](https://dial2vincent.github.io/) | 
| Jenkins | CICD | | [more...](https://github.com/dial2vincent/Simple-DevOps-Project/tree/master/Jenkins) | 
| Kubernetes | Container Orchestrator | |[More..](https://github.com/dial2vincent/lab) |
| Linux | CentOS Oracle RHEL Ubuntu | | [More..](https://github.com/dial2vincent/lab)] |
| Packer | Image builder | You can build standard images with a consistent configuration for things like patching, time, networking, security, and compliance to be maintained across environments. For example, an infrastructure or a security team can use Packer to build images that are then shared with other groups to provide baseline builds that force cross-organizational standards. | [more...](https://dial2vincent.github.io/) |
| Puppet | Configuration pull based | | [More..](https://github.com/dial2vincent/lab) |
| Elastic | Elasticsearch Kibana | |  [Read more...](https://dial2vincent.github.io/) | 
| Terraform | Provisioning | Terraform is a tool for building, changing, and versioning infrastructure safely and efficiently. Terraform can manage existing and popular service providers and custom in-house solutions. Configuration files describe to Terraform the components needed to run a single application or your entire data center. |[More..](https://github.com/dial2vincent/lab) |
| Vagrant | Virtual Build | |[More..](https://github.com/dial2vincent/lab) |
| WSL | Windows Subsystem Linux |  | [More..](https://github.com/dial2vincent/lab) |

--- 
## Projects
| Name | Type | Description | Last Update |
| ----------- | ----------- | ----------- | ----------- |
| Simple DevOps Project | Public | [Read more...](https://github.com/dial2vincent/Simple-DevOps-Project) | 2023 |
| 3-tier-architecture | Public | [Read more...](https://github.com/dial2vincent/3-tier-architecture) | 2023 |
| Infrastructure As Code (IaC) | Private | [Read more...](https://github.com/dial2vincent/iac) | 2023 |

--- 
## Build your lab environment 
- Host Operating System: Linux (CentOS, Oracle Linux, RHEL, Ubuntu, Windows, Mac)
- Virtual Machines: AWS, Azure, Hyper-V, Virtual Box
- Cloud: AWS, [Azure](https://github.com/dial2vincent/azure)
- Private: [Metro](https://github.com/dial2vincent/dial2me) [Resume](https://github.com/dial2vincent/dial2git)

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
- Ansible control node: utility, ubuntu
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
 - office (Ubuntu, DESKTOP-198)
 
[^1]: Location: AWS, Hosts: myvm, myweb 
[^2]: Location: Windows 2012 Hyper-v
[^3]: Location: B

## Tracking the CHANGELOG.md
1. Ansible control node: ubuntu | Hosts: ubuntu1, ubuntu2, ~~node2~~
2. Puppet master: oracle | puppet client: oracle1, oracle2 
3. Web Server: myweb, Requirement Tools: Tomcat server,
  
## Tips & Notes
### How to find your Github Repo Size
- Opening your Account Settings → Repositories (https://github.com/settings/repositories), and the repository size is displayed next to its designation.
