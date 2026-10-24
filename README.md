

# Dockerized Web Application

[![Docker Build CI](https://github.com/jyothisjose9a/dockerized-web-app/actions/workflows/docker-build.yml/badge.svg)](https://github.com/jyothisjose9a/dockerized-web-app/actions/workflows/docker-build.yml)

## Overview
A beginner-friendly DevOps portfolio project that demonstrates how to containerize and serve a static HTML website using Docker and Nginx.

## Technologies Used
- Linux (Ubuntu)
- Docker
- Nginx
- HTML and CSS
- Git and GitHub

## Project Structure
```text
dockerized-web-app/
├── Dockerfile
├── index.html
├── .dockerignore
└── README.md
```

## Prerequisites
- Docker installed and running

## Build the Docker Image
```bash
docker build -t my-docker-web-app:1.0 .
```

## Run the Container
```bash
docker run -d -p 8080:80 --name my-web-container my-docker-web-app:1.0
```

Open http://localhost:8080 in your browser.

## Verify the Application
```bash
docker ps
curl http://localhost:8080
docker logs my-web-container
```

## Stop and Restart the Container
```bash
docker stop my-web-container
docker start my-web-container
```

## Clean Up
```bash
docker stop my-web-container
docker rm my-web-container
```


