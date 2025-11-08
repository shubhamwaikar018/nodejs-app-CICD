
 # 🚀Node.js CI/CD Pipeline using Jenkins on AWS EC2

This project demonstrates a **Node.js web application** deployed automatically using a **Jenkins CI/CD pipeline** hosted on an **AWS EC2 instance**.

---

 # Project Overview

- **Language/Framework:** Node.js (Express.js)
- **CI/CD Tool:** Jenkins
- **Server:** AWS EC2 (Ubuntu)
- **Version Control:** GitHub
- **Build Tool:** npm (depending on project setup)
- **Pipeline Type:** Declarative Jenkins Pipeline (Jenkinsfile)

---

## AWS EC2 Instance (Ubuntu)
![](./images/Screenshot%202025-11-08%20101422.png)
## ⚙️ Prerequisites

Before you begin, make sure you have the following installed:
- **Node.js & npm**
- **Jenkins Server** (installed and running on EC2)
- **Git** (for fetching code from GitHub)

---

## 🖥️ Jenkins Setup on EC2

### 1️⃣ Install Jenkins
```bash
sudo apt update
sudo apt install jenkins -y
sudo systemctl enable jenkins
sudo systemctl start jenkins
```
## Jenkinsfile

✅ Updated the Jenkinsfile in VS Code to automate the build and deployment process of the Node.js application.
![](./images/Screenshot%202025-11-08%20101452.png)


## 🔗Connect GitHub Repository

1) Go to Jenkins Dashboard → New Item → Pipeline

2) Add your GitHub Repository URL

3) Select "Pipeline script from SCM"

4) Choose Git
```bash
Paste your repository URL
https://github.com/shubhamwaikar018/nodejs-app-CICD.git
```

5) Set branch (main)

### Image of connect github repository
![](./images/Screenshot%202025-11-08%20101409.png)


## Output
✅ Successfully built and deployed the Node.js application using Jenkins on AWS EC2. The pipeline ran smoothly, completing all stages — checkout, clone, upload, install, and start — without errors. 
The screenshot shows the final successful build execution, confirming the CI/CD setup is working perfectly.

![](./images/Screenshot%202025-11-08%20101340.png)

![](./images/Screenshot%202025-11-08%20101606.png)

## Conclusion
The Node-App-Deployment project helped to set up a complete CI/CD process for a Node.js application using Jenkins on an AWS EC2 server. The pipeline automatically fetched the latest code from GitHub, built the project, and deployed it without manual steps. Overall, this setup made the deployment process quicker, more consistent, and easier to manage, while improving the speed and reliability of updates.