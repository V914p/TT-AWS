---
title: "Worklog Tuần 3"
date: 2026-05-04
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---


### Objective of Worklog:

* Hiểu kiến trúc và workflow triển khai VPC trên AWS
* Học cách tạo và cấu hình EC2 Instance
* Thực hành SSH remote access và cấu hình bảo mật
* Làm quen với quản lý tài nguyên computer trên cloud

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| 2 | - Thực hành: Tạo IAM Group <br><br> - Gán quyền <br><br> - Thêm user vào group | 04/05/2026 | 04/05/2026 | <https://000002.awsstudygroup.com/vi/3-aws-role/> |
| 3 | - Chuyển đổi IAM Roles: Tạo Operator User, Đăng Nhập, Chuyển đổi Roles | 05/05/2026 | 05/05/2026 | <https://000002.awsstudygroup.com/vi/4-switch-roles/> |
| 4 | - Chuẩn bị các bước để làm lab3<br> - Tạo VPC, Subnet, Internet Gateway, Route Table, SG, VPC Flow Logs | 06/05/2026 | 06/05/2026 | <https://000003.awsstudygroup.com/vi/3-prerequisite/> |
| 5 | - Triển khai EC2 Instances<br> - EC2, Kiểm tra, NAT Gateway, Sử RA, AWS SMSM, CloudWatch | 07/05/2026 | 07/05/2026 | <https://000003.awsstudygroup.com/vi/4-createec2server/> |
| 6 | - Cấu Hình VPN<br> - Tạo VPN, Kết nối VPN | 08/05/2026 | 08/05/2026 | <https://000003.awsstudygroup.com/vi/5-vpnsitetosite/> |


### Kết quả đạt được tuần 3:

* Hoàn thành các bài thực hành liên quan đến IAM.
* Tạo các IAM Group, User và Role.
* Thực hành chuyển đổi vai trò IAM giữa các người dùng.
* Hiểu được kiến trúc cơ bản của Amazon VPC.
* Tạo các thành phần mạng cốt lõi:
  * VPC.
  * Public và Private Subnet.
  * Internet Gateway.
  * Route Tables.
  * Security Groups.
  * VPC Flow Logs.
* Triển khai các EC2 Instance bên trong VPC.
* Học hiểu mục đích cơ bản của NAT Gateway, SSM, và CloudWatch.
* Thực hành cấu hình kết nối VPN Site-to-Site.
* Cải thiện hiểu biết về mạng AWS và truy cập từ xa an toàn.

### Ảnh chụp và Minh chứng:

#### VPC Configuration

![VPC Setting](/images/1-Worklog/1.3-Week3/VPC%20Setting.PNG)

![VPC](/images/1-Worklog/1.3-Week3/VPC.PNG)

![Subnet](/images/1-Worklog/1.3-Week3/Subnet.PNG)

#### Internet Gateway & Route Tables

![Internet Gateway](/images/1-Worklog/1.3-Week3/InternetGateway.PNG)

![Attach Internet Gateway](/images/1-Worklog/1.3-Week3/AttachInternetGateway.PNG)

![Route Table](/images/1-Worklog/1.3-Week3/RouteTable.PNG)

![Route Table Private](/images/1-Worklog/1.3-Week3/RouteTable-Private.PNG)

#### Security Groups

![Security Group Public Subnet](/images/1-Worklog/1.3-Week3/SG-PublicSubnet.PNG)

![Security Group Private Subnet](/images/1-Worklog/1.3-Week3/SG-PrivateSubnet.PNG)

![Security Group VPC Endpoints](/images/1-Worklog/1.3-Week3/SG-VPCEnpoints.PNG)

#### EC2 Instances

![EC2 Public](/images/1-Worklog/1.3-Week3/EC2%20Public.PNG)

![EC2 Public + Private](/images/1-Worklog/1.3-Week3/EC2%20Public%20+%20Private.PNG)

![EC2 Instance VPN](/images/1-Worklog/1.3-Week3/EC2%20Instance%20VPN.PNG)

#### NAT Gateway

![NAT Gateway](/images/1-Worklog/1.3-Week3/NAT%20Gateway.PNG)

#### VPC Flow Logs

![VPC Flow Logs](/images/1-Worklog/1.3-Week3/VPC%20Flow%20Logs.PNG)

![CloudWatch VPC Flow Logs](/images/1-Worklog/1.3-Week3/CloudWatchVPCFlowLogs.PNG)

#### VPN Configuration

![VPN Connection](/images/1-Worklog/1.3-Week3/VPN%20Connection.PNG)

![VPN Subnet](/images/1-Worklog/1.3-Week3/VPN%20Subnet.PNG)

![Virtual Private Gateway](/images/1-Worklog/1.3-Week3/Virtual%20Private%20Gateway.PNG)

![Customer Gateway](/images/1-Worklog/1.3-Week3/Customer%20Gateway.PNG)

![ASG VPN](/images/1-Worklog/1.3-Week3/ASG%20VPN.PNG)

![Route Table VPN](/images/1-Worklog/1.3-Week3/RouteTableVPN.PNG)

![Route Table VPN Route Propagation](/images/1-Worklog/1.3-Week3/RouteTableVPNRoutePropa.PNG)

![Route Table VPN Route Propagation Public](/images/1-Worklog/1.3-Week3/RouteTableVPNRoutePropaPublic.PNG)

![Route Table VPN Subnet](/images/1-Worklog/1.3-Week3/RouteTableVPNSubnet.PNG)

#### Session Manager & Transit Gateway

![Session Manager](/images/1-Worklog/1.3-Week3/Session%20Manager.PNG)

![Connect To EC2 Transit Gateway](/images/1-Worklog/1.3-Week3/Connect%20To%20EC2%20TransitGateway.PNG)

![Connect To EC2 Transit Gateway 1](/images/1-Worklog/1.3-Week3/Connect%20To%20EC2%20TransitGateway1.PNG)

#### Monitoring & CloudWatch

![CloudWatch Alarm](/images/1-Worklog/1.3-Week3/CloudWatchAlarm.PNG)

![Dashboard](/images/1-Worklog/1.3-Week3/DashBoard.PNG)

#### Connectivity Testing

![Public EC2 Connection Check](/images/1-Worklog/1.3-Week3/Public%20EC2%20Connection%20Check.PNG)

![Public + Private EC2 Connection Checking](/images/1-Worklog/1.3-Week3/Public%20+%20Private%20EC2%20Connection%20Checking.PNG)

![Reachability Analyzer](/images/1-Worklog/1.3-Week3/Reachability%20Analyzer.PNG)

![Reachability Analyzer 01](/images/1-Worklog/1.3-Week3/Reachability%20Analyzer01.PNG)

![Reachability Analyzer 02](/images/1-Worklog/1.3-Week3/Reachability%20Analyzer02.PNG)

#### Key Management

![Key Check](/images/1-Worklog/1.3-Week3/key%20check.PNG)

![Key Check 2](/images/1-Worklog/1.3-Week3/key%20check2.PNG)

#### VPC Endpoints

![Endpoint SSM](/images/1-Worklog/1.3-Week3/EnpointSSM.PNG)


