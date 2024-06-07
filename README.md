
# What is  My Lab
> My lab is to experiment and learn—critical tasks for pursuing cloud computing, Linux, learning new automation tools for setting up the cloud environment, improving DevOps work skills, or experimenting with cloud services.

![Tools on WSL](wsl.PNG)

--- 
## Table of content  
| Name | Type | Description | Link | 
| ----------- | ----------- | ----------- | ----------- |
| Terraform | Infrastructure Provisioning | Terraform is a tool for building, changing, and versioning infrastructure safely and efficiently. Terraform can manage existing and popular service providers and custom in-house solutions. Configuration files describe to Terraform the components needed to run a single application or your entire data center. |[more..](https://github.com/dial2vincent/Terraform-Tutorial) |
| Ansible | Configuration (push-based) | Ansible is a configuration management tool that can configure Linux devices and Windows, and it’s agentless. The Playbooks used to configure systems are YAML format files that are easily read and write a playbook on how the system should be set up. |[more..](https://github.com/dial2vincent/lab/blob/master/content/ansible.md) |
| Puppet | Configuration (pull-based) | | [more..](https://github.com/dial2vincent/lab/blob/master/content/puppet.md) |
| Bash | Linux | |  [more...](https://github.com/dial2vincent/bash) | 
| Docker | Container | | [more..](https://github.com/dial2vincent/lab) |
| Elastic | Elasticsearch Kibana | |  [more...](https://dial2vincent.github.io/) | 
| Git | Version Control | | [more..](https://github.com/dial2vincent/lab) |
| Github | Git remote repository | |  [more...](https://dial2vincent.github.io/) | 
| Jenkins | CICD | | [more...](https://github.com/dial2vincent/Simple-DevOps-Project/tree/master/Jenkins) | 
| Kubernetes | Container Orchestrator | |[more..](https://github.com/dial2vincent/lab) |
| Linux | CentOS Oracle RHEL Ubuntu | | [more..](https://github.com/dial2vincent/lab) |
| Packer | Image builder | You can build standard images with a consistent configuration for things like patching, time, networking, security, and compliance to be maintained across environments. For example, an infrastructure or a security team can use Packer to build images that are then shared with other groups to provide baseline builds that force cross-organizational standards. We use a Continuous Integration/Continuous Deployment (CI/CD) approach to deploy new Amazon EC2 images. Packer builds Amazon Machine Images (AMIs) using Ansible, Terraform uses those AMIs when hosts and services are built, and Ansible runs again to provide final configuration and to keep our hosts correctly configured.  | [more...](https://dial2vincent.github.io/) |


| Vagrant | Virtual Build | |[more..](https://github.com/dial2vincent/lab) |
| WSL | Windows Subsystem Linux |  | [more..](https://github.com/dial2vincent/lab) |

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
