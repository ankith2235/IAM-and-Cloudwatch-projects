# AWS IAM & CloudWatch Projects – 5 Assignments

This repository contains projects completed as part of my Cloud & DevOps training, focusing on **AWS Identity and Access Management (IAM)** and **Amazon CloudWatch**.  
The objective was to improve account security, user access control, cost monitoring, and infrastructure observability for an enterprise use case.

---

## 🔹 Project 1: CloudWatch Billing and EC2 CPU Alarms
**Problem Statement:**  
Monitor AWS account costs and EC2 performance to proactively detect issues and control expenses.

**Tasks Performed:**
1. Created a **CloudWatch Billing Alarm** that triggers when estimated AWS charges exceed **$500**
2. Created a **CloudWatch Alarm** for an EC2 instance when **CPU utilization exceeds 65%**
3. Configured an **SNS topic** to send notifications when the alarm threshold is crossed

**Outcome:**  
Implemented cost and performance monitoring with real-time alerting.

---

## 🔹 Project 2: CloudWatch Dashboard for EC2 Monitoring
**Problem Statement:**  
Provide a centralized view to monitor EC2 instance performance.

**Tasks Performed:**
1. Created a **CloudWatch Dashboard**
2. Added widgets to monitor:
   - EC2 CPU Utilization
   - Network In and Network Out metrics
3. Customized the dashboard for a specific EC2 instance

**Outcome:**  
Enabled visual monitoring of EC2 performance metrics from a single dashboard.

---

## 🔹 Project 3: IAM Policies and Group-Based Access Control
**Problem Statement:**  
Control user access using fine-grained IAM policies and groups.

**Tasks Performed:**

### Policy 1:
- Full access to **Amazon S3**
- Permission to **only create EC2 instances**
- Full access to **Amazon RDS**

### Policy 2:
- Full access to **CloudWatch** and **Billing**
- Read-only (list) access to **EC2** and **S3**

**Implementation:**
1. Created both IAM policies
2. Attached **Policy 1** to the **Dev Team**
3. Attached **Policy 2** to the **Ops Team**

**Outcome:**  
Implemented least-privilege access using IAM policies and groups.

---

## 🔹 Project 4: IAM Role Creation and Role Switching
**Problem Statement:**  
Allow specific users to assume a role with elevated permissions.

**Tasks Performed:**
1. Created an **IAM Role** with:
   - Full access to **VPC**
   - Full access to **DynamoDB**
2. Configured the role trust policy to allow **user1** and **user2**
3. Logged in as **user1** and successfully **assumed the role** to verify permissions

**Outcome:**  
Validated secure access escalation using IAM roles and role switching.

---

## 🔹 Project 5: IAM Users and Groups Setup
**Problem Statement:**  
Organize users into teams with appropriate access control.

**Tasks Performed:**
1. Created IAM users:
   - Dev1
   - Dev2
   - Test1
   - Test2
2. Created IAM groups:
   - Dev Team
   - Ops Team
3. Added:
   - **Dev1 and Dev2** to **Dev Team**
   - **Dev1, Test1, and Test2** to **Ops Team**

**Outcome:**  
Structured IAM users and groups to reflect organizational roles.

---

## 🛠 AWS Services Used
- Amazon Identity and Access Management (IAM)
- Amazon CloudWatch
- Amazon SNS
- Amazon EC2
- AWS Billing & Cost Management
- AWS Management Console

---

## 🎯 Summary
These projects provided hands-on experience with AWS security and monitoring services, including IAM users, groups, policies, roles, CloudWatch alarms, dashboards, and billing alerts. The work focused on implementing secure access control, cost monitoring, and operational visibility in a real-world enterprise scenario.
