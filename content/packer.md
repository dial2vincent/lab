# Packer
## Packer install on Ubuntu
[Reference URL](https://developer.hashicorp.com/packer/tutorials/docker-get-started/docker-get-started-build-image)

~~~
wget -O- https://apt.releases.hashicorp.com/gpg | sudo gpg --dearmor -o /usr/share/keyrings/hashicorp-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list
sudo apt update && sudo apt install packer
~~~

## Packer build an image
- `mkdir packer_tutorial`
- `cd packer_tutorial`
- `nano docker-ubuntu.pkr.hcl`
- Add content below to build an Ubuntu Docker image.
~~~
packer {
  required_plugins {
    docker = {
      version = ">= 1.0.8"
      source = "github.com/hashicorp/docker"
    }
  }
}

source "docker" "ubuntu" {
  image  = "ubuntu:jammy"
  commit = true
}

build {
  name    = "learn-packer"
  sources = [
    "source.docker.ubuntu"
  ]
}
~~~
- `packer init .` Initialize Packer configuration
- `packer fmt .` Format your template. Packer will print out the names of the files it modified.
- `packer validate .` Validate your template
- `packer build docker-ubuntu.pkr.hcl` Build Packer image
- `docker images`
---

