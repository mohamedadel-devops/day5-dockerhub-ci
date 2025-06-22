# DockerHub CI/CD with GitHub Actions & EC2

This project demonstrates a complete CI/CD pipeline using **GitHub Actions**, **DockerHub**, and **AWS EC2**. It builds a Docker image for a sample web app, pushes it to DockerHub, and deploys it to a remote EC2 instance.

---

## 🚀 Features

- GitHub Actions CI pipeline
- Docker image build & push to DockerHub
- Deployment to AWS EC2
- Public access via EC2 public IP

---

## 🔧 Tech Stack

- Docker
- GitHub Actions
- DockerHub
- AWS EC2 (Ubuntu)
- Flask (Python-based web app)

---

## 📁 Project Structure

.
├── app.py
├── Dockerfile
├── requirements.txt
└── .github
└── workflows
└── dockerhub.yml
---

## ⚙️ GitHub Actions Workflow

On every push to the `main` branch:
1. GitHub Actions builds the Docker image using the provided Dockerfile.
2. It logs in to DockerHub using stored secrets.
3. It pushes the image to [DockerHub](https://hub.docker.com/u/mohammedrs).

---

## 🔗 DockerHub Image

```bash
docker pull mohammedrs/day5-dockerhub-ci
docker run -d -p 5000:5000 mohammedrs/day5-dockerhub-ci

🌍 Live App
Accessible via:

http://34.219.157.83:5000

👤 Author
Mohamed Adel Asar
