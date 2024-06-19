




## MicroK8s Installation on WSL
Installing MicroK8s on Windows Subsystem for Linux (WSL) is a good way to practice Kubernetes commands, as it provides a lightweight, easy-to-install version of Kubernetes that is well-suited for local development and testing. Here are the steps to install MicroK8s on WSL:
### Steps
1. Install WSL and a Linux Distribution:
If you haven't already installed WSL and a Linux distribution, you need to do that first. Follow these steps:

Open PowerShell as an administrator and run:
`wsl --install`
- Restart your computer if prompted.
- After the restart, you can install your preferred Linux distribution (e.g., Ubuntu) from the Microsoft Store.
2. Update and Upgrade the Linux Distribution:
Open your WSL terminal (e.g., Ubuntu) and update the package lists and upgrade installed packages:

~~~
sudo apt update
sudo apt upgrade -y
~~~
3. Install MicroK8s:

- Install snapd if it’s not already installed:
`sudo apt install snapd`\
- Install MicroK8s using snap:
`sudo snap install microk8s --classic`
4. Add Your User to the microk8s Group:
Add your user to the microk8s group to avoid using sudo for MicroK8s commands:

~~~
sudo usermod -a -G microk8s $USER
newgrp microk8s
~~~
5. Enable Core Kubernetes Services:
Enable essential services such as the DNS and dashboard:

`microk8s enable dns dashboard`
6. Set Up kubectl Command:
Create an alias for kubectl to use MicroK8s' version of the command:
`alias kubectl='microk8s kubectl'`
7. Verify the Installation:
Check the status of MicroK8s to ensure it's running correctly:

`microk8s status --wait-ready` 
8. Test kubectl Commands:
You can now start practicing Kubernetes commands. For example:

~~~
kubectl get nodes
kubectl create deployment nginx --image=nginx
kubectl get pods
~~~
By following these steps, you can set up MicroK8s on WSL and start practicing Kubernetes commands in a local development environment. If you encounter any issues, feel free to ask for further assistance!
