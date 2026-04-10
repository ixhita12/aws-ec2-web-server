# 🌐 AWS EC2 Web Server Deployment

## 📌 Project Overview
This project demonstrates the deployment of a web server using Amazon Web Services (AWS) EC2. The objective was to gain hands-on experience with cloud infrastructure, Linux-based server management, and basic networking concepts by hosting a live webpage on a virtual machine.

---

## 🚀 Technologies Used
- Amazon Web Services (AWS EC2)
- Ubuntu (Linux)
- Nginx Web Server

---

## ⚙️ Implementation Steps

### 1. EC2 Instance Setup
- Launched an EC2 instance using Ubuntu AMI
- Selected t2.micro instance type (Free Tier eligible)
- Created and downloaded a key pair for secure access

### 2. Network Configuration
- Enabled SSH (Port 22) for secure remote access
- Enabled HTTP (Port 80) to allow public web traffic

### 3. Server Access
- Connected to the instance using EC2 Instance Connect (browser-based terminal)

### 4. Web Server Installation
Installed Nginx using the following commands:

```bash
sudo apt update
sudo apt install nginx -y

### 5. Service Management
- Started the Nginx service:
```bash
sudo systemctl start nginx

Enabled auto-start on reboot:
sudo systemctl enable nginx
###6. Verification
-Checked service status:
```bash
sudo systemctl status nginx
-Verified server locally:
```bash
curl localhost
-Accessed the web server using Public IPv4 address in a browser
