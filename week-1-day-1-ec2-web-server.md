# Week 1 Day 1 — AWS EC2 Static Web Server Deployment

## Overview

This project demonstrates the deployment of a basic web server on AWS using EC2, Apache HTTP Server, and Security Groups. The objective was to understand foundational cloud concepts including compute provisioning, network security, and service configuration.

---

## Architecture

Internet → AWS Security Group → EC2 Instance (Amazon Linux 2) → Apache (httpd) → Static HTML Page

---

## AWS Services Used

- Amazon EC2 (t2.micro)
- AWS Security Groups
- Amazon Linux 2 AMI
- SSH Key Pair Authentication
- Apache HTTP Server (httpd)

---

## Implementation Steps

1. Launched EC2 instance using Amazon Linux 2 AMI (t2.micro)
2. Configured Security Group:
   - Allowed SSH (port 22) from my IP
   - Allowed HTTP (port 80) from 0.0.0.0/0
3. Connected to instance via SSH using key pair authentication
4. Installed Apache HTTP Server:
   ```bash
   sudo yum install -y httpd