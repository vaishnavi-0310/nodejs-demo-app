# Node.js CI/CD Demo App

## Objective
Automate code deployment using GitHub Actions.

## Tools
- Node.js
- Docker
- GitHub Actions

## What I Did
- Created a Node.js web app using Express.
- Added simple Jest tests.
- Created a Dockerfile to containerize the app.
- Configured GitHub Actions workflow (`.github/workflows/main.yml`) to:
  - Run tests on push to `main`.
  - Build Docker image.
  - Push image to Docker Hub.

## Usage Instructions
1. Clone repo: `git clone https://github.com/vaishnavi-0310/nodejs-demo-app.git`
2. Run locally:
   ```bash
   npm ci
   npm test
   node index.js


## Commands for Setup, Docker, and GitHub Push
1. Create project folder
   mkdir nodejs-demo-app
   cd nodejs-demo-app

2. Initialize Git and npm
   git init
   npm init -y

3. Install Dependencies
   npm install express
   npm install --save-dev jest

4. Run locally
   npm ci
   npm test
   node index.js

5. Docker Build and Run Locally
   docker build -t nodejs-demo-app:local .
   docker run -p 3000:3000 --rm nodejs-demo-app:local

6. Push to GitHub (after creating remote repository)
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/<your-github-username>/nodejs-demo-app.git
   git push -u origin main

