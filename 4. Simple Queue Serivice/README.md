# 📬 AWS SQS Internship Project – Amazon Simple Queue Service

## 📖 Project Overview

As part of my summer internship focused on **AWS Cloud Computing**, this project explores the usage of **Amazon Simple Queue Service (SQS)** — a fully managed message queuing service that enables **asynchronous decoupling of microservices**, distributed systems, and serverless applications.

The project demonstrates how to create and configure SQS queues, integrate with Amazon SNS and AWS Lambda, send and receive messages, and implement real-time processing using event-driven architecture.

---

## 🔑 What is Amazon SQS?

Amazon SQS offers:
- Secure and durable message queuing
- Decoupling between producers and consumers
- FIFO and Standard queues
- Dead-letter queue support
- Serverless integration with AWS Lambda
- Seamless SNS topic subscriptions

---

## 💼 Key Features Implemented

### ✅ Queue Creation & Configuration
- Created a **Standard Queue** with:
  - Visibility timeout
  - Message retention period
  - Delivery delay
  - Max message size
  - Receive wait time
- Server-Side Encryption (SSE) with AWS-managed keys

### 📩 SNS Integration
- Created an **SNS FIFO topic**
- Subscribed the queue to the SNS topic
- Published structured messages from SNS to SQS
- Verified message delivery to SQS

### ⚙️ Message Sending & Receiving
- Sent test messages directly to the queue
- Observed and validated message availability
- Received messages using "Send and receive message" feature

### ⚡ AWS Lambda Trigger
- Created a Lambda function triggered by SQS events
- Assigned **AmazonSQSFullAccess** role to Lambda
- Verified automatic message processing
- Deleted Lambda function after testing

### 🗑️ Resource Cleanup
- Deleted SNS topic, Lambda function, and SQS queue with appropriate confirmations

---

## 📂 Project Structure

```bash
aws-sqs-project/
├── 📄 README.md
├── 📄 Simple_Queue_Service.pdf       # Detailed guide with screenshots
└── 📁 screenshots/                   # Visual references
