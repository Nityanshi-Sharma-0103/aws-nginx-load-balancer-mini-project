# AWS Nginx Load Balancer Mini Project

## Overview
This mini project demonstrates how to deploy a highly available **Nginx web application** on AWS using **multiple EC2 instances** behind a **Classic Load Balancer**.

This project was built as part of hands-on DevOps learning.

---

## Architecture
User traffic is routed through a Load Balancer which distributes requests across two EC2 instances.

User  
↓  
Classic Load Balancer  
↓  
EC2 Instance 1 (Nginx)  
EC2 Instance 2 (Nginx)

---

## Technologies Used
- AWS EC2
- Classic Load Balancer
- Amazon Linux 2023
- Nginx
- Linux
- MobaXterm (SSH)

---

## Implementation Steps
1. Launched two EC2 instances using Amazon Linux.
2. Connected to both instances using SSH via MobaXterm.
3. Installed and started Nginx on both instances.
4. Created custom HTML pages.
5. Created a Classic Load Balancer.
6. Attached both EC2 instances to the load balancer.
7. Configured health checks.
8. Verified traffic distribution using the Load Balancer DNS.

---

## Commands Used
```bash
sudo yum install nginx
sudo systemctl start nginx
sudo systemctl enable nginx
cd /usr/share/nginx/html
vi index.html
