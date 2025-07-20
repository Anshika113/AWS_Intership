# 📣 AWS SNS Internship Project – Amazon Simple Notification Service

## 📖 Project Overview

This project is part of my **AWS Internship**, focusing on Amazon **Simple Notification Service (SNS)** — a fully managed messaging service that enables **pub-sub (publish-subscribe)** communication between applications and users.

The goal of this hands-on module was to understand and implement **message delivery mechanisms** using topics, subscriptions, and protocols like **Email** and **SMS**. It also includes managing and verifying subscriptions and sending real-time notifications from a publisher to a subscriber endpoint.

---

## 🔑 What is Amazon SNS?

Amazon SNS allows:
- **Publishers** to send messages to a **topic**
- **Subscribers** to receive messages via supported **protocols** (e.g., Email, SMS, Lambda, HTTP)
- **Asynchronous, decoupled communication** across microservices or apps

---

## 💼 Key Features Covered

### ✅ Creating Topics
- Standard Topic creation (used for Email and SMS notifications)
- Naming conventions and topic ARN configuration

### 📩 Email Subscription
- Email subscription setup to an SNS topic
- Confirmation via email
- Publishing messages to email subscribers

### 📱 SMS Subscription
- Adding and verifying phone numbers for SMS delivery
- Publishing SMS notifications to verified numbers
- Language selection for verification

### 🗑️ Managing Resources
- Deleting subscriptions
- Deleting topics with confirmation phrase `"delete me"`

---

## 📂 Project Structure

```bash
aws-sns-project/
├── 📄 README.md
├── 📄 Simple_Notification_Service.pdf  
└── 📁 screenshots/                     
