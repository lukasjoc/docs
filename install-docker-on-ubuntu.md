# Install Docker and Docker-Compose on Ubuntu >=20.04

## Update Deps
```bash
sudo apt update; sudo apt upgrade
````

## Get Repository
```bash
sudo apt install apt-transport-https ca-certificates curl gnupg-agent software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
```

## Docker/Docker-Compose Install
```bash
sudo apt install docker-ce docker-ce-cli containerd.io
sudo apt-get install python3 python3-pip
pip -v install docker-compose
```

## Add user to docker group
```bash
sudo systemctl status docker
sudo usermod -aG docker "YOUR_USER"
```
