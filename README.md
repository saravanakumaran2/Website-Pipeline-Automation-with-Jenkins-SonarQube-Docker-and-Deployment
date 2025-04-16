# Website Pipeline Automation with Jenkins + SonarQube + Docker + Deployment
 
This is my end-to-end automation project where I combined **Jenkins**, **SonarQube**, **Docker**, and **remote server deployment** — all in one pipeline.  

---

## What I Did in This Project

- Created a `Jenkinsfile` to define the full CI/CD pipeline
- Integrated **SonarQube** to do code quality checks (static code analysis)
- Used **Docker** to build a Docker image of the website/app
- Pushed the Docker image to **Docker Hub**
- Deployed the Docker container to a **remote server** using SSH
- Automated everything using **pipeline stages** in Jenkins

---

## Pipeline Breakdown (Stage-by-Stage)

1. **Clone Repo** – Jenkins pulls code from GitHub
2. **SonarQube Scan** – Runs quality analysis and shows report in Jenkins
3. **Docker Build** – Builds a Docker image from `Dockerfile`
4. **Docker Push** – Pushes the image to your Docker Hub account
5. **Deploy Remotely** – Connects to remote server via SSH and runs the container

---

## What’s in the Repo

```bash
.
├── Jenkinsfile              
├── Dockerfile              
├── sonar-project.properties 
└── README.md               
```

---

## How to Use It

1. Set up Jenkins with:
   - Docker
   - SonarQube plugin
   - SSH and Docker Hub credentials
2. Create a Pipeline project in Jenkins
3. Link it to this GitHub repo

---

## Why I Built This

I wanted to learn **how real DevOps pipelines work** — from scanning code to deploying it live.  
This project helped me understand how tools like Jenkins, Docker, and SonarQube work **together**.

---

