# 🗂️ AWS S3 Internship Project – Amazon Simple Storage Service (S3)

## 📖 Project Overview

As part of my summer internship focused on **cloud computing with AWS**, this project dives deep into **Amazon S3 (Simple Storage Service)** — one of the most essential services for storing and retrieving any amount of data from anywhere on the web.

The goal of this project is to explore **object storage management** using S3 through hands-on tasks such as creating buckets, managing permissions, uploading files, enabling version control, using presigned URLs, and configuring storage classes.

This project was carried out using the **AWS Free Tier** and is aimed at mastering **real-world storage use cases** such as file hosting, secure file sharing, and backup/versioning workflows.

---

## 🧠 Key Concepts & Features Covered

### ✅ Bucket Creation & Configuration
- General Purpose Bucket setup
- Region selection (e.g., Mumbai)
- Object ownership management (ACL enabled/disabled)
- Public vs. private access configuration

### 🔐 Access Control
- Public access with ACL
- Private access with presigned URLs
- Blocking/unblocking public access
- Acknowledging risks during public bucket creation

### 📁 Object Management
- Uploading multiple files via AWS Console
- Creating and editing `.html` and `.txt` files
- Updating and overwriting existing objects
- Using AWS S3's console interface for file access

### 🔗 Presigned URLs
- Generating secure time-limited links for file access
- Sharing private files securely without changing bucket permissions

### 🧬 Versioning & Object Lock
- Enabling versioning at bucket level
- Tracking object versions after file updates
- Restoring previous file versions
- Object Lock for compliance and data immutability
- Configuring retention mode (`Governance` or `Compliance`)

### 💾 Storage Class Configuration
- Understanding S3 storage tiers:
  - Standard
  - Standard-IA (Infrequent Access)
  - Intelligent-Tiering (optional for advanced use)
- Editing object storage class after upload
- Managing storage cost with efficient classification

---

## 📂 Folder Structure

```bash
aws-s3-project/
├── 📄 README.md               # This documentation
├── 📄 S3_Project_Report.pdf   # Detailed step-by-step project walkthrough
└── 📁 screenshots/            # (Optional) Images for hosting/demo
