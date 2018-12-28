# How to install docker "CE" on "Ubuntu 18.04.1 LTS

# Follow this steps: https://docs.docker.com/install/linux/docker-ce/ubuntu/#install-using-the-repository

# Resume:

1) sudo apt-get remove docker docker-engine docker.io
2) sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    software-properties-common
3) curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
4) sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"
5) sudo apt-get update
6) sudo apt-get install docker-ce

# Verify:

1) sudo docker run hello-world
