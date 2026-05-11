---
title: "Week 3 Worklog"
date: 2026-05-04
weight: 3
chapter: false
pre: "<b>1.3.</b>"
---

## 🎯 Week 3 Objectives

- Understand AWS EC2 architecture and deployment workflow
- Learn how to launch and configure an EC2 instance
- Practice SSH remote access and security configuration
- Gain experience managing compute resources in AWS

---

## 📅 Weekly Plan & Tracking

| Day | Date       | Tasks                                                                 | Status | Notes |
|-----|-----------|----------------------------------------------------------------------|--------|------|
| Mon | 04/05/2026 | - Study AWS EC2 overview <br> - Learn Instance Types, AMI, EBS       | ⬜ | |
| Tue | 05/05/2026 | - Learn EC2 pricing models <br> - Understand Security Group & Key Pair | ⬜ | |
| Wed | 06/05/2026 | - Practice launching EC2 instance <br> - Configure Amazon Linux 2    | ⬜ | |
| Thu | 07/05/2026 | - Configure Security Group rules <br> - Enable SSH access via port 22 | ⬜ | |
| Fri | 08/05/2026 | - Connect to EC2 using SSH <br> - Verify instance status and monitoring | ⬜ | |

---

## ☁️ AWS EC2 Deployment Process

### Step 1: Launch EC2 Instance

- Open AWS Console → EC2 Dashboard
- Select:
  - Amazon Linux 2 AMI
  - t2.micro instance type (Free Tier)
- Configure storage and network settings

---

### Step 2: Configure Security Group

Inbound Rules:

| Type | Protocol | Port | Source |
|------|----------|------|--------|
| SSH  | TCP      | 22   | My IP |

Purpose:
- Allow secure remote SSH access to EC2

---

### Step 3: Create Key Pair

- Create `.pem` key pair
- Download and securely store private key

Used for:
- SSH authentication
- Secure remote login

---

### Step 4: Connect via SSH

```bash
ssh -i mykey.pem ec2-user@public-ip