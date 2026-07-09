# AWS DevOps Engineer Intern Assignment

## Objective

Deploy a simple static website on an AWS EC2 Ubuntu instance using Nginx, perform basic Linux administration tasks, manage the project using Git & GitHub, and document the complete deployment process.

---

# AWS Services Used

* Amazon EC2 (Ubuntu Server)
* Security Groups
* Additional Security Group (Bonus)
* VPC (Default)
* Public IPv4 Address

---

# EC2 Configuration

* **Instance Type:** t3.small
* **Operating System:** Ubuntu
* **Web Server:** Nginx
* **SSH Access:** Port 22
* **HTTP Access:** Port 80
* **HTTP Access:** Port 8080

---

# Linux Commands Used

```bash
sudo apt update
sudo apt upgrade -y

sudo apt install nginx -y

sudo systemctl status nginx
sudo systemctl restart nginx
sudo systemctl enable nginx

df -h
free -m
ps -ef
top
htop
```

---

# Website Deployment

* Installed Nginx on the Ubuntu EC2 instance.
* Removed the default Nginx welcome page.
* Created a custom `index.html` page containing:

  * Name
  * College
  * Branch
  * Email
  * Current Date
* Replaced the default Nginx page with the custom HTML page.
* Verified that the website was accessible using the EC2 Public IP address.

---

# Git & GitHub

## Git Commands

```bash
git init
git add .
git commit -m "New Add"
git branch -M main
git remote add origin <My Repo Url>
git push -u origin main
```

---

# Project Structure

```text
AWS-DevOps-Intern-Assignment/
│── index.html
│── README.md
│── Report.pdf
│── Screenshots/
│   ├── EC2.png
│   ├── Security_Group.png
│   ├── SSH.png
│   ├── Nginx.png
│   ├── Hosting.png
│   ├── Docker_HelloWorld.png
│   └── New_Security_Group.png
```

---

# Bonus Task 1 – Docker Installation

Docker was installed on the EC2 instance and verified successfully by running the `hello-world` container.

## Commands Used

```bash
sudo apt-get update
sudo apt-get install docker.io -y
sudo systemctl start docker
sudo systemctl enable docker
sudo docker run hello-world
```

**Result:** Docker was installed successfully and the `hello-world` container executed successfully.

---

# Bonus Task 2 – Additional Security Group

Created an additional Security Group for practice and attached it to the EC2 instance.

Configuration:

| Rule | Port | Source               |
| ---- | ---- | -------------------- |
| SSH  | 22   | My IP                |
| HTTP | 80   | Anywhere (0.0.0.0/0) |
| HTTP | 8080 | Anywhere (0.0.0.0/0  |

---

# Deliverables

* EC2 Public IP
* EC2 Dashboard Screenshot
* Security Group Screenshot
* SSH Login Screenshot
* Nginx Installation Screenshot
* Website Screenshot
* GitHub Repository
* PDF Documentation
* Docker Bonus Screenshot
* Additional Security Group Screenshot

---

# Learnings

* Launched and configured an AWS EC2 instance.
* Configured Security Groups for secure network access.
* Connected to the EC2 instance using SSH.
* Installed and managed the Nginx web server.
* Hosted a static website on AWS.
* Performed basic Linux administration tasks.
* Managed project files using Git and GitHub.
* Installed Docker and verified the installation by running the `hello-world` container.
* Created and attached an additional Security Group to the EC2 instance.

---

# Time Taken

Approximately **1 hours**.

---

# Author

**Name:** Manoj Gavhane

**College:** Sinhgad Institute of Technology, Pune

**Branch:** Computer Engineering

**Email:** [manojgavhane1812@example.com](mailto:your-email@example.com)
**Website:** www.manojkgavhane.co.in
