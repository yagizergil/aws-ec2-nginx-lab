# AWS EC2 Nginx Lab

This project demonstrates a basic AWS EC2 setup with an Nginx web server to understand
fundamental cloud infrastructure concepts such as compute, networking, and security.

---

## 🧱 Architecture

- AWS EC2 (Ubuntu 24.04 LTS)
- Security Group (SSH & HTTP)
- Public IPv4
- Nginx web server

---

## 🚀 What I Built

- Launched an EC2 instance using Ubuntu 24.04 LTS
- Connected to the instance via SSH
- Installed and started Nginx web server
- Exposed the service to the internet using Security Group rules

---

## 🧠 What I Learned

- A running service can still be unreachable due to network restrictions
- AWS Security Groups act as a virtual firewall
- Opening port 80 is required for HTTP traffic
- Linux services can be managed using systemctl

---

## 🧪 Verification Steps

```bash
sudo systemctl status nginx
Expected output:

arduino
Kodu kopyala
Active: active (running)
Access via browser:

cpp
Kodu kopyala
http://<EC2_PUBLIC_IP>
💥 What Broke (On Purpose)
Removing port 80 from the Security Group blocked external access

Re-adding the rule restored connectivity

📌 Notes
A typo in the package name (ngnix vs nginx) caused installation failure

This lab was created as part of a cloud engineering learning path
