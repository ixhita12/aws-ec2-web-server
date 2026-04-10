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

---

### 2. Network Configuration
- Enabled SSH (Port 22) for secure remote access  
- Enabled HTTP (Port 80) to allow public web traffic  

---

### 3. Server Access
- Connected to the instance using EC2 Instance Connect (browser-based terminal)  

---

### 4. Web Server Installation

```bash
sudo apt update
sudo apt install nginx -y
```

---

### 5. Service Management

```bash
sudo systemctl start nginx
sudo systemctl enable nginx
```

---

### 6. Verification

```bash
sudo systemctl status nginx
curl localhost
```

- Accessed the web server using Public IPv4 address in a browser  

---

## 📸 Output
Successfully deployed a live web server and accessed the default Nginx welcome page through the EC2 instance's public IP.

---

## 💡 Key Learnings
- Understanding how cloud-based virtual machines (EC2) are provisioned and managed  
- Hands-on experience with Linux command-line operations  
- Configuring security groups to control inbound traffic  
- Managing services using systemctl  
- Deploying and verifying a web server in a cloud environment  

---

## ⚠️ Note
The EC2 instance was terminated after completing the project to avoid unnecessary charges under AWS Free Tier.

---

## 📈 Future Improvements
- Deploy a custom HTML/CSS website  
- Configure a domain name and HTTPS  
- Integrate with GitHub for automated deployments  
