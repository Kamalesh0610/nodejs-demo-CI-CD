# Node.js CI/CD Demo App

This repository demonstrates a simple Node.js web application with automated deployment using GitHub Actions and Docker.

## 🚀 Project Overview

- **Objective:** Automate code deployment using a CI/CD pipeline.
- **Tools Used:** GitHub, GitHub Actions, Node.js, Docker, DockerHub.

## 📦 Features

- Sample Express.js web server ([index.js](index.js))
- Automated build, test, and Docker image deployment via GitHub Actions ([.github/workflows/main.yml](.github/workflows/main.yml))
- Dockerfile for containerization ([Dockerfile](Dockerfile))

## ⚙️ CI/CD Pipeline

The pipeline is defined in [.github/workflows/main.yml](.github/workflows/main.yml):

1. **Trigger:** On push to `main` branch.
2. **Steps:**
   - Checkout code
   - Set up Node.js
   - Install dependencies
   - Run tests
   - Build Docker image
   - Login to DockerHub
   - Push image to DockerHub

## 🐳 Docker

To build and run locally:

```sh
docker push kamalesh0610/nodejs-demo-app:latest
docker run -p 3000:3000 kamalesh0610/nodejs-demo-app:latest
```

## 📝 How It Works

- On every push to `main`, GitHub Actions runs the pipeline.
- The app is built, tested, and a Docker image is pushed to DockerHub.

## 📂 Repository Structure

- `index.js` — Express.js server
- `Dockerfile` — Container setup
- `.github/workflows/main.yml` — CI/CD workflow
- `package.json` — Project metadata and dependencies
- `ScreenShot/` — Screenshots 


## 📸 Screenshots

> - Running the Production Build via serve
![image alt](https://github.com/Kamalesh0610/nodejs-demo-CI-CD/blob/main/Screenshot/01.png)


> - Running the Production Build via serve
![image alt](https://github.com/Kamalesh0610/nodejs-demo-CI-CD/blob/main/Screenshot/02.png)


> - Running the Production Build via serve
![image alt](https://github.com/Kamalesh0610/nodejs-demo-CI-CD/blob/main/Screenshot/03.png)

## 🏁 Getting Started

1. Clone the repo
2. Install dependencies: `npm install`
3. Start locally: `npm start`
4. View at [http://localhost:3000](http://localhost:3000)

## 🔒 Secrets

- Store DockerHub credentials as GitHub repository secrets: `DOCKER_USERNAME`, `DOCKER_PASSWORD`.

## 📤 Submission

Submit your GitHub repo link as per the guidelines.

---

> - Running the Production Build via serve
![image alt](https://github.com/Kamalesh0610/Brain-Tasks-App/blob/main/Screenshot/01.png)
