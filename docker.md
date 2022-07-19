sudo apt-get update && \
    sudo apt-get install \
    ca-certificates \
    curl \
    gnupg \
    lsb-release -y


curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg


sudo apt-get update && sudo apt-get install docker-ce docker-ce-cli containerd.io -y


sudo docker run hello-world


sudo usermod -a -G docker ubuntu
