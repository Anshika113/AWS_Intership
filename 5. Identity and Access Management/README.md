# 🛡️ AWS IAM Internship Project – Identity and Access Management

## 📖 Project Overview

This project was completed as part of my AWS internship, focusing on **Identity and Access Management (IAM)**, a foundational security service offered by Amazon Web Services. The goal was to explore the **creation and management of users, groups, and policies**, and to understand how IAM controls access to AWS resources in a secure and scalable way.

This hands-on project demonstrates:
- User authentication and authorization workflows
- Granular access control using policies
- Real-world implementation of permission delegation via IAM

---

## 🔑 What is AWS IAM?

**AWS Identity and Access Management (IAM)** enables you to:
- Securely manage **who can access** your AWS resources
- Define **what actions** they can perform
- Control access using **policies**, **roles**, and **groups**
- Monitor and audit access for **compliance and security**

---

## 🧰 Key Features Covered

### 👤 IAM Users
- Created users with custom login credentials
- Configured sign-in permissions for AWS Management Console
- Provided selective access (e.g., EC2-only access)

### 👥 User Groups
- Grouped users for collective permission management
- Assigned permissions to groups using AWS-managed and custom policies
- Added multiple users into groups with centralized control

### 📜 Policies
- Explored AWS-managed policies
- Created custom policies using the IAM Policy Builder
- Assigned policies to users and groups

### 🔒 Permissions Control
- Attached direct permissions to users
- Limited access to specific services (e.g., EC2, SNS)
- Verified access denial on unauthorized services

### 🗑️ Resource Cleanup
- Deleted users, groups, and policies via the IAM console

---

## 📂 Project Structure

```bash
aws-iam-project/
├── 📄 README.md
├── 📄 IAM_Project_Report.pdf          # Full step-by-step documentation
└── 📁 screenshots/                    # Visuals
