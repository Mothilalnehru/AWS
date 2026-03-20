\# 🚀 AWS EC2 Setup Guide



\## 📌 What is EC2?

Amazon EC2 (Elastic Compute Cloud) is a service that provides virtual servers in the cloud.



\---



\## 🛠️ Steps to Launch an EC2 Instance



1\. Login to AWS Console

2\. Go to EC2 Dashboard

3\. Click \*\*Launch Instance\*\*



\---



\## ⚙️ Configuration



\### 1. Name

\- MyEC2Instance



\### 2. AMI (Operating System)

\- Ubuntu Server 22.04 LTS



\### 3. Instance Type

\- t2.micro (Free Tier)



\### 4. Key Pair

\- Create new key pair

\- Download `.pem` file



\### 5. Network Settings

\- Allow:

&#x20; - SSH (port 22)

&#x20; - HTTP (port 80)



\---



\## 🚀 Launch Instance

Click \*\*Launch Instance\*\*



\---



\## 🔗 Connect to EC2



\### Using SSH:

```bash

ssh -i key.pem ubuntu@your-public-ip



🌐 Host a Simple Web Server 

sudo apt update

sudo apt install apache2 -y

sudo systemctl start apache2



👉 Open browser and visit:

http://your-public-ip



✅ Result

&#x20;Apache default webpage is displayed in browser

&#x20;EC2 instance is successfully running a web server



&#x20;⚠️ Common Errors

🔹 Permission Denied (SSH Error)

chmod 400 key.pem





🔹 Connection Timeout

Check Security Group

Make sure:

Port 22 (SSH) is allowed

Port 80 (HTTP) is allowed

Verify correct Public IP





🎯 Conclusion

Successfully:

Launched an EC2 instance

Connected using SSH

Installed and started Apache server

Hosted a simple web page

This demonstrates basic cloud server setup using AWS EC2.





