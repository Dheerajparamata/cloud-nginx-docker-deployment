# Deploy an Nginx Website Using Docker on Google Cloud Platform

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

- GCP VM Instance
- Docker Installation
- Docker Version
- Docker Container Running
- Browser Output
- curl localhost Output

## Author

**Dheeraj Paramata**
