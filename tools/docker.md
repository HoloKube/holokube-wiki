# Docker

In the [docker site](https://docs.docker.com/engine/install/) you will be able to find all platforms installation guide.
or follow the bellow commands for Ubuntu Linux distribution.

### Install using the repository

Uninstall older versions of Docker
```bash
 sudo apt-get remove docker docker-engine docker.io containerd runc
```

#### Install using the repository

##### Update the apt package index and install packages to allow apt to use a repository over HTTPS:
```bash
 sudo apt-get update
 
 sudo apt-get install \
     apt-transport-https \
     ca-certificates \
     curl \
     gnupg-agent \
     software-properties-common
```

##### Add Docker’s official [GPG key](https://en.wikipedia.org/wiki/GNU_Privacy_Guard):
```bash
 curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
```
##### Verify that you now have the key with the fingerprint 9DC8 5822 9FC7 DD38 854A  E2D8 8D81 803C 0EBF CD88
```bash
 sudo apt-key fingerprint 0EBFCD88
 
 pub   rsa4096 2017-02-22 [SCEA]
       9DC8 5822 9FC7 DD38 854A  E2D8 8D81 803C 0EBF CD88
 uid           [ unknown] Docker Release (CE deb) <docker@docker.com>
 sub   rsa4096 2017-02-22 [S]
```

##### Use the following command to set up the stable repository.
```bash
 sudo add-apt-repository \
    "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
    $(lsb_release -cs) \
    stable"
```

##### Update the apt package index, and install the latest version of Docker Engine and containerd
```bash
 sudo apt-get update
 sudo apt-get install docker-ce docker-ce-cli containerd.io
```
