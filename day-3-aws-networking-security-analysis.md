# Week 1 Day 3 — AWS Networking & Security Group Traffic Flow Analysis

## Overview

This exercise focused on understanding how network traffic flows through AWS infrastructure and how Security Groups control access to cloud resources.

The analysis was based on a previously deployed EC2 instance hosting a static Apache web server.

No new infrastructure was deployed during this exercise.

---

# Objective

Understand how:

- Public internet traffic reaches AWS EC2 instances
- Security Groups function as stateful firewalls
- Public IP exposure works in AWS
- Misconfigured network rules impact service availability

---

# Architecture Flow

```text
Client Device (Laptop)
        ↓
Public Internet
        ↓
AWS Public IP Address
        ↓
Internet Gateway
        ↓
VPC (Virtual Private Cloud)
        ↓
Subnet
        ↓
Security Group (Firewall Rules)
        ↓
EC2 Instance (Amazon Linux 2)
        ↓
Apache HTTP Server (httpd)