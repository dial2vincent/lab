
# What is  My Lab
> My lab is to experiment and learn—critical tasks for pursuing cloud computing, Linux, learning new automation tools for setting up the cloud environment, improving DevOps work skills, or experimenting with cloud services.

![Tools on WSL](wsl.PNG)

--- 
## Table of content  
| Name | Type | Description | Link | 
| ----------- | ----------- | ----------- | ----------- |
| Terraform | Infrastructure Provisioning | Terraform is a tool for building, changing, and versioning infrastructure safely and efficiently. Terraform can manage existing and popular service providers and custom in-house solutions. Configuration files describe to Terraform the components needed to run a single application or your entire data center. |[more..](https://github.com/dial2vincent/Terraform-Tutorial) |
| Packer | Image builder | You can build standard images with a consistent configuration for things like patching, time, networking, security, and compliance to be maintained across environments. For example, an infrastructure or a security team can use Packer to build images that are then shared with other groups to provide baseline builds that force cross-organizational standards. We use a Continuous Integration/Continuous Deployment (CI/CD) approach to deploy new Amazon EC2 images. Packer builds Amazon Machine Images (AMIs) using Ansible, Terraform uses those AMIs when hosts and services are built, and Ansible runs again to provide final configuration and to keep our hosts correctly configured.  | [more...](https://github.com/dial2vincent/lab/blob/master/content/packer.md) |
| Vagrant | Virtual Build | Vagrant is an open-source tool that helps us to automate the creation and management of Virtual Machines. |[more..](https://github.com/dial2vincent/lab/blob/master/content/vagrant.md) |
| Ansible | Configuration (push-based) | Ansible is a configuration management tool that can configure Linux devices and Windows and is agentless. The Playbooks used to configure systems are YAML format files that are easily read and write a playbook on how the system should be set up. |[more..](https://github.com/dial2vincent/lab/blob/master/content/ansible.md) |
| Puppet | Configuration (pull-based) | Puppet, you define the desired state of the systems in your infrastructure that you want to manage. | [more..](https://github.com/dial2vincent/lab/blob/master/content/puppet.md) |
| Jenkins | CICD | Jenkins is a tool used for automation, and it is an open-source server that allows all developers to build, test, and deploy software. | [more...](https://github.com/dial2vincent/Simple-DevOps-Project/tree/master/Jenkins) | 
| Docker | Container | Docker is a tool for running your applications inside containers, which package all the dependencies and code your app needs to run into a single file. | [more..](https://github.com/dial2vincent/lab/blob/master/content/docker.md) |
| Kubernetes | Container Orchestrator | Kubernetes is a portable, extensible, open-source platform for managing containerized workloads and services, that facilitates both declarative configuration and automation. |[more..](https://github.com/dial2vincent/lab/blob/master/content/k8s.md) |
| Git | Version Control | Git is a distributed version control system that tracks versions of files. | [more..](https://github.com/dial2vincent/lab/blob/master/content/git.md) |
| Github | Git remote repository | GitHub is a cloud-based platform where you can store, share, and work together with others to write code. |  [more...](https://github.com/dial2vincent/lab/blob/master/content/github.md) | 
| Linux | CentOS Oracle RHEL Ubuntu | Linux is an open-source operating system (OS). An operating system is the software that directly manages a system’s hardware and resources, like CPU, memory, and storage.  | [more..](https://github.com/dial2vincent/lab/blob/master/content/linux.md) |
| WSL | Windows Subsystem Linux | Windows Subsystem For Linux (WSL) is a tool provided by Microsoft to run Linux natively on Windows. | [more..](https://github.com/dial2vincent/lab/blob/master/content/wsl.md) |
| Bash | Linux | Bash is a command-line interpreter or Unix Shell |  [more...](https://github.com/dial2vincent/bash) [shell](https://github.com/dial2vincent/lab/blob/master/content/bash.md)| 
--- 
## Sample Projects
| Name | Type | Description | Link |
| ----------- | ----------- | ----------- | ----------- |
| Simple DevOps Project | Public | CICD with Jenkins, Ansible, Docker, Kubernetes | [Read more...](https://github.com/dial2vincent/Simple-DevOps-Project) | 
| Hello World | Public | CICD with Jenkins, Ansible, Docker, Kubernetes | [Read more...](https://github.com/dial2vincent/hello-world) | 
| 3-tier-architecture | Public | Installation of Terraform on AWS and install EC2 on AWS | [Read more...](https://github.com/dial2vincent/3-tier-architecture) |
| Infrastructure As Code (IaC) | Private | Build Lab Environment | [Read more...](https://github.com/dial2vincent/iac) |
--- 

## Lab environment 
- Cloud: AWS, Azure
- Virtual Machines: AWS, Azure, Hyper-V, Virtual Box
- Host Operating System: Linux (CentOS, Oracle Linux, RHEL, Ubuntu), Windows, Mac


## Tracking the CHANGELOG.md
1. Ansible control node: ubuntu | Hosts: ubuntu1, ubuntu2, ~~node2~~
2. Puppet master: oracle | puppet client: oracle1, oracle2 
3. Web Server: myweb, Requirement Tools: Tomcat server,
  
## Tips & Notes
### How to find your Github Repo Size
- Opening your Account Settings → Repositories (https://github.com/settings/repositories), and the repository size is displayed next to its designation.
