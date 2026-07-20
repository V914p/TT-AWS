---
title: "Worklog Tuần 5"
date: 2026-05-18
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---


### Objective of Worklog:

* Tìm hiểu tổng quan về Amazon EC2 trên AWS
* Học cách triển khai và quản lý EC2 Instance
* Thực hành cấu hình Security Group, Key Pair và SSH
* Làm quen với workflow quản trị Linux Server trên cloud
* Tìm hiểu monitoring và quản lý tài nguyên EC2

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| 2 | - Tìm hiểu tổng quan Amazon EC2<br> - Học EC2 Instance Types<br> - Tìm hiểu AMI và EBS | 18/05/2026 | 18/05/2026 |  |
| 3 | - Tạo Linux EC2 Instance<br> - Cấu hình Key Pair<br> - Tìm hiểu Pricing EC2 | 19/05/2026 | 19/05/2026 |  |
| 4 | - Cấu hình Security Group<br> - Mở SSH Port 22<br> - Quản lý Inbound & Outbound Rules | 20/05/2026 | 20/05/2026 |  |
| 5 | - Kết nối SSH tới EC2 Linux<br> - Kiểm tra môi trường Linux Server<br> - Thực hành command cơ bản | 21/05/2026 | 21/05/2026 |  |
| 6 | - Monitoring EC2 bằng CloudWatch<br> - Kiểm tra CPU, Network, Status Check<br> - Quản lý trạng thái Instance | 22/05/2026 | 22/05/2026 |  |


### Kết quả đạt được tuần 5:

* Kiến thức đạt được
* Amazon EC2 architecture
* Linux Server deployment workflow
* SSH remote access
* Security Group management
* CloudWatch monitoring cơ bản
* Quản lý tài nguyên compute trên AWS
* Khó khăn
* Lỗi SSH Permission denied
* Cấu hình Security Group chưa chính xác
* Quản lý quyền file .pem
* Troubleshoot kết nối EC2
* Hướng cải thiện
* Học Elastic IP
* Deploy Web Application lên EC2
* Học Docker trên Linux Server
* Tìm hiểu Auto Scaling và Load Balancer

### Ảnh chụp và Minh chứng:

#### EC2 Instances

![EC2 Instance Linux](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/EC2-Instance-Linux.PNG)

![EC2 Instance Window](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/EC2-Instance-Window.PNG)

![Linux Remote EC2](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/Linux-Remote-EC2.PNG)

![Window Remote EC2](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/Window-Remote-EC2.PNG)

![Window Remote EC2 2](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/Window-Remote-EC2-2.PNG)

#### VPC & Subnets

![Linux VPC](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/Linux-VPC.PNG)

![Window VPC](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/Window-VPC.PNG)

![Subnet](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/Subnet.PNG)

![Subnet Window](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/Subnet-Window.PNG)

#### Security Groups

![Security Group All](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/Security-Group-All.PNG)

![Security Group Linux](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/Security-Group-Linux.PNG)

![Security Group Window](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/Security-Group-Window.PNG)

![Linux Allow Rule](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/Linux-Allow-Rule.PNG)

#### MariaDB Setup

![MariaDB PW Reset](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/MariaDB-PWreset.PNG)

![PHP DB Create](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/PHP-DBcreate.PNG)

![ADD DB](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/ADD-DB.PNG)

![DB Success Add](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/DB-SuccessAdd.PNG)

#### Database Connectivity

![ConnectDB OnLinux](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/ConnectDB-OnLinux.PNG)

![ConnectDB OnLinux After](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/ConnectDB-OnLinux-After.PNG)

![FE ADD DB Linux](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/FE-ADD-DB-Linux.PNG)

![FE DB Linux](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/FE-DB-Linux.PNG)

#### PHP MyAdmin

![PHP MyAdmin After](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/PHP-MyAdmin-After.PNG)

![PHP Test Web](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/PHP-TestWeb.PNG)

![FE HomePage DB Linux](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/FE-HomePage-DB-Linux.PNG)

![FE EDIT DB Linux](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/FE-EDIT-DB-Linux.PNG)

![FE SearchUser DB Linux](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/FE-SearchUser-DB-Linux.PNG)

![Delete PHP File](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/Delete-PHPFile.PNG)

#### Node.js Setup

![NPM INIT](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/NPM-INIT.PNG)

![npm local setup](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/npm-local-settup.PNG)

![Nodejs Setting On Linux](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/Nodejs-Setting-On-Linux.PNG)

![WindowInstance NodeJS Setup](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/WindowInstance-NodeJS-Settup.PNG)

![WindowInstance NodeJS Setup Checkout](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/WindowInstance-NodeJS-Settup-Checkout.PNG)

#### XAMPP Setup (Windows)

![XAMMP SETUP Window](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/XAMMP-SETTUP-Window.PNG)

#### Custom AMI & Snapshots

![Custom AMI](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/Custom-AMI.PNG)

![Instance from Custom AMI](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/Instance-from-Custom-AMI.PNG)

![Window Snapshot](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/Window-Snapshot.PNG)

#### Linux Environment

![Linux Enabled and Setting](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/Linux-EnabledandSetting.PNG)

![Linux Check](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/IPV4-Linux-Check.PNG)

![DNS Linux Check](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/DNS-Linux-Check.PNG)

![DNS LambServer Check](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/DNS-LambServerCheck.PNG)

#### Windows Instance Management

![Window Instance Change](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/Window-Instance-Change.PNG)

![Window Instance Change 2](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/Window-Instance-Change-2.PNG)

![Window Instance Change 3](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/Window-Instance-Change-3.PNG)

![Window Instance Stopped](/TT-AWS/images/1-Worklog/1.5-Week5/Lab04/Window-Instance-Stopped.PNG)

### Lab05: RDS và Setup Database

#### Cấu hình VPC cho Database

![VPC created](/TT-AWS/images/1-Worklog/1.5-Week5/Lab05/VPC-created.PNG)

#### Security Groups cho RDS

![Security created](/TT-AWS/images/1-Worklog/1.5-Week5/Lab05/Security-created.PNG)

![SG RDS Created](/TT-AWS/images/1-Worklog/1.5-Week5/Lab05/SG-RDS-Created.PNG)

#### RDS Database Subnet Group

![DB Subnet Group](/TT-AWS/images/1-Worklog/1.5-Week5/Lab05/DB-Subnet-Group.PNG)

#### EC2 Instance để truy cập Database

![EC2 Instance Created](/TT-AWS/images/1-Worklog/1.5-Week5/Lab05/EC2-Instance-Created.PNG)

#### Kiểm tra Kết nối

![Connect EC2 Success](/TT-AWS/images/1-Worklog/1.5-Week5/Lab05/Connect-EC2-Success.PNG)

![Done Setting MobaXterm](/TT-AWS/images/1-Worklog/1.5-Week5/Lab05/Done-Setting-MobaXterm.PNG)


