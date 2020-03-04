# ubuntu-setup-env

## Install VSCode
## Install Nodejs
## Config terminal with oh-my-zsh
## Install Docker
- ``sudo apt update``
- ``sudo apt install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg-agent \
    software-properties-common``
- ``curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -``
- ``sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"``
- ``sudo apt update``
- ``sudo apt-get install docker-ce docker-ce-cli containerd.io``

Test running ``hello-world`` image:
- ``sudo docker run hello-world``
Enable Docker to run as non-root

- ``sudo groupadd docker``
- ``sudo usermod -aG docker $USER``
