# vagrant-docker

Install Docker on Ubuntu

```
# https://docs.docker.com/engine/install/ubuntu/
# https://docs.docker.com/engine/install/linux-postinstall/

# Update the apt package index and install packages to allow apt to use a repository over HTTPS:
$ sudo apt-get update

$ sudo apt-get -y install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg-agent \
    software-properties-common

# Add Docker’s official GPG key:
$ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

# Use the following command to set up the stable repository.
$ sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"

# Update the apt package index, and install the latest version of Docker Engine and containerd
$ sudo apt-get update
$ sudo apt-get -y install docker-ce docker-ce-cli containerd.io docker-compose
```
