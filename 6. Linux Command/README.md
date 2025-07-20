# 🐧 Linux Commands in AWS EC2 – Internship Project

## 📖 Project Overview

This project focuses on the practical use of **Linux commands within an AWS EC2 environment**, completed during my AWS internship. By launching an **Amazon Linux EC2 instance**, I practiced a wide variety of essential system-level tasks like file operations, user management, directory navigation, software installation, permission control, and more using the Linux terminal.

The hands-on experience was aimed at equipping myself with core skills needed for managing cloud-based Linux servers in real-world DevOps, system administration, and cloud engineering roles.

---

## 🧰 Tools & Technologies Used

- **Amazon Web Services (AWS)**
  - EC2 (Elastic Compute Cloud)
  - Amazon Linux OS
- **Linux Shell (Bash)**
- **SSH (EC2 Connect Console)**

---

## 🧑‍💻 Key Skills Practiced

### 🔹 Instance Launch & Connection
- Launching EC2 instance with Amazon Linux
- Connecting via EC2 Connect
- Switching to root user using `sudo su`

### 🔹 File Operations
| Command | Function |
|--------|----------|
| `touch file1` | Create empty file |
| `cat > file1` | Create file with content |
| `cat file1` | View file content |
| `cat >> file1` | Append to file |
| `rm file1` | Remove file with confirmation |
| `rm -f file1` | Force delete file |
| `rm -rvf file*` | Recursive delete with pattern |

### 🔹 Directory Operations
| Command | Function |
|--------|----------|
| `mkdir my` | Create directory |
| `mkdir my/abc` | Create nested directory |
| `cd ..` | Go back |
| `cd /var/www/html` | Navigate to path |
| `pwd` | Print working directory |
| `ls`, `ls -a`, `ll`, `ll -a` | List files, including hidden |

### 🔹 File Editing
- Using `vim` for interactive editing:
  - `i` to insert
  - `ESC` + `:wq` to save and quit
- Using `cat` to input/update content

### 🔹 User Management
| Command | Function |
|--------|----------|
| `useradd user1` | Add new user |
| `su user1` | Switch to user1 |

### 🔹 Software Management
| Command | Description |
|--------|-------------|
| `yum update -y` | Update system packages |
| `yum install httpd -y` | Install Apache Web Server |
| `systemctl start httpd` | Start Apache service |
| `systemctl status httpd` | Check service status |

### 🔹 File Permissions
| Command | Description |
|--------|-------------|
| `chmod 111 file1` | Execute only |
| `chmod 222 file1` | Write only |
| `chmod 444 file1` | Read only |
| `chmod 777 file1` | Full permissions (rwx) |
| `chown` and `chgrp` | (Additional permission management if needed) |

---

## 📂 Project Structure

```bash
aws-linux-commands/
├── 📄 README.md
├── 📄 linux.pdf                 # Full step-by-step walkthrough
└── 📁 screenshots/             # Terminal outputs, EC2 dashboards
