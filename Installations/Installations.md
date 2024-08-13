# Docker Installation

To install Jenkins on Debian/Ubuntu systems, follow these steps:

```bash
# Add Docker's official GPG key:
sudo apt-get update -y
sudo apt-get install ca-certificates curl
sudo install -m 0755 -d /etc/apt/keyrings
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
sudo chmod a+r /etc/apt/keyrings/docker.asc

# Add the repository to Apt sources:
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update -y
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
sudo docker run hello-world
```
## script copied from 
``` bash
    https://docs.docker.com/engine/install/ubuntu/

```


# Jenkins Installation

To install Jenkins on Debian/Ubuntu systems, follow these steps:

```bash
sudo apt update
sudo apt install openjdk-17-jdk
java -version
sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]" \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt-get update
sudo apt-get install jenkins
```
## script copied from 
``` bash
    https://www.jenkins.io/doc/book/installing/linux/#debianubuntu

```
# Nodejs and Npm installation

To install Jenkins on Debian/Ubuntu systems, follow these steps:

```bash
sudo apt update -y
curl -fsSL https://deb.nodesource.com/setup_current.x | sudo -E bash - && sudo apt-get install -y nodejs


```

#Apache2 server installation

To install apache2 server systems, follow these steps:

```bash
sudo apt update -y
sudo apt install apache2 -y

```
