# DevOps CI/CD Pipeline Project 

## What this project is about

In this project, I built a complete DevOps workflow from scratch.

I started with a simple HTML app and then step by step turned it into a real deployment setup using Docker, GitHub Actions, and AWS EC2.

Now whenever I push code to GitHub, the app is automatically rebuilt, pushed to Docker Hub, and deployed on my EC2 server.

---

## Tech I used

* Linux (Ubuntu)
* Docker
* Nginx
* GitHub Actions
* AWS EC2
* Docker Hub

---

## How the whole flow works

```text
Code → GitHub → GitHub Actions → Docker Hub → EC2 → Live App
```

---

## What happens when I push code

1. I push code to GitHub
2. GitHub Actions starts automatically
3. It builds a Docker image of my app
4. The image is pushed to Docker Hub
5. GitHub connects to my EC2 server using SSH
6. EC2 pulls the latest image
7. The old container is stopped and removed
8. A new container runs with the updated version

---

## What I did step-by-step

* Created a simple HTML app
* Wrote a Dockerfile and ran it locally
* Used Nginx inside the container
* Set up GitHub Actions for automation
* Connected Docker Hub to store images
* Launched an EC2 instance on AWS
* Installed Docker on EC2
* First deployed manually
* Then automated deployment using CI/CD

---

## How to run it locally

```bash
docker build -t devops-app .
docker run -p 8080:80 devops-app
```

Then open: http://localhost:8080

---

## Deployment

The app is deployed on AWS EC2 and updates automatically whenever I push new changes.

---

## Screenshot of output

<img width="971" height="417" alt="image" src="https://github.com/user-attachments/assets/1be98a95-7772-429b-b31c-9566beb0f3a1" />

---

## What I learned

* How Docker works in a real project
* How CI/CD pipelines actually run
* How to connect GitHub with a remote server
* How deployments are handled in practice

---

## Note

This project is part of my DevOps learning journey.
I focused on understanding each step instead of just copying a setup.
