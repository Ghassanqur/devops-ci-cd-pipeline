# Docker DevOps Project

## Overview
Containerized a static web application using Docker and Nginx.

## What I Did
- Created a Dockerfile
- Built Docker image
- Ran container

## Project Files
- index.html
- Dockerfile

## Build Image
docker build -t devops-app .

## Run Container
docker run -d -p 8080:80 devops-app

## Result
App running at:
http://localhost:8080
