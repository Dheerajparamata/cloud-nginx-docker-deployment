# Cloud Nginx Docker Deployment

Deploying an Nginx web server inside a Docker container on a Google Cloud Platform (GCP) Virtual Machine.

## Project Overview

This project demonstrates how to deploy an Nginx web server inside a Docker container on a Google Cloud Platform (GCP) Virtual Machine.

## Technologies Used

- Google Cloud Platform (GCP)
- Compute Engine
- Debian 12
- Docker
- Docker Hub
- Nginx
- Linux

## Project Architecture

```text
Internet
   │
   ▼
Google Cloud VM
   │
   ▼
Docker Container
   │
   ▼
Nginx Web Server
```

## Commands Used

```bash
sudo apt update
sudo apt install docker.io -y

sudo systemctl enable docker
sudo systemctl start docker

docker --version

sudo docker pull nginx

sudo docker run -d --name mynginx -p 80:80 nginx

sudo docker ps

curl http://localhost
```

## Result

- Successfully deployed an Nginx container.
- Verified Docker container status.
- Accessed the website using the VM's public IP.
- Confirmed deployment through a web browser.

  ## Screenshots

### 1. GCP VM Instance
![GCP VM Instance](screenshots/1.%20vm-instance.png)

### 2. Docker Installation
![Docker Installation](screenshots/2.%20docker-install%20pg1.png)

### 3. Docker Version
![Docker Version](screenshots/3.%20docker-version.png)

### 4. Docker Container Running
![Docker Container Running](screenshots/4.%20docker-ps.png)

### 5. Browser Output
![Browser Output](screenshots/5.%20nginx-browser.png)

### 6. curl localhost Output
![curl localhost Output](screenshots/6.%20curl-localhost.png)


## Author

**Dheeraj Paramata**
