---
title: "Week 3 Worklog"
date: 2026-05-04
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---


### Objective of Worklog:

* Understand AWS VPC architecture and deployment workflow.
* Learn how to create and configure EC2 instances.
* Practice SSH remote access and security configuration.
* Become familiar with managing compute resources on the cloud.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ---- | ---------- | --------------- | ------------------ |
| 2 | - Practice: Create an IAM Group <br> - Assign permissions <br> - Add users to the group | 05/04/2026 | 05/04/2026 | <https://000002.awsstudygroup.com/vi/3-aws-role/> |
| 3 | - Switch IAM Roles <br> - Create an Operator User <br> - Sign in and switch roles | 05/05/2026 | 05/05/2026 | <https://000002.awsstudygroup.com/vi/4-switch-roles/> |
| 4 | - Prepare for Lab 3 <br> - Create VPC, Subnet, Internet Gateway, Route Table, Security Group, and VPC Flow Logs | 05/06/2026 | 05/06/2026 | <https://000003.awsstudygroup.com/vi/3-prerequisite/> |
| 5 | - Deploy EC2 Instances <br> - Test EC2 connectivity <br> - Learn NAT Gateway, SSM, and CloudWatch basics | 05/07/2026 | 05/07/2026 | <https://000003.awsstudygroup.com/vi/4-createec2server/> |
| 6 | - Configure Site-to-Site VPN <br> - Create VPN connection <br> - Test VPN connectivity | 05/08/2026 | 05/08/2026 | <https://000003.awsstudygroup.com/vi/5-vpnsitetosite/> |

### Week 3 Achievements:

* Completed IAM-related practice labs.
* Created IAM groups, users, and roles.
* Practiced switching IAM roles between users.
* Understood the basic architecture of Amazon VPC.
* Created core networking components:
  * VPC.
  * Public and private subnets.
  * Internet Gateway.
  * Route Tables.
  * Security Groups.
  * VPC Flow Logs.
* Deployed EC2 instances inside the VPC.
* Learned the basic purpose of NAT Gateway, SSM, and CloudWatch.
* Practiced configuring a Site-to-Site VPN connection.
* Improved understanding of AWS networking and secure remote access.

### Screenshots and Evidence:

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


