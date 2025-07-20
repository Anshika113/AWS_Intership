# 🐧 Linux Commands in AWS EC2 Instance

## 📘 Introduction

In Amazon Web Services (AWS), Linux commands are essential for managing and interacting with EC2 instances—virtual machines running in the cloud. After connecting to a Linux instance via SSH, users use Linux commands to perform tasks like:

* Navigating directories (`cd`, `ls`)
* Managing files (`cp`, `mv`, `rm`, `nano`, `vim`)
* Installing software (`yum`, `apt-get`)
* Monitoring system performance (`top`, `htop`, `df`, `free`)
* Managing permissions and users (`chmod`, `chown`, `adduser`)
* Starting and stopping services (`systemctl`, `service`)
* Transferring files (`scp`, `rsync`)
* Running scripts and automating tasks (`bash`, `cron`)

These commands enable users to configure servers, deploy applications, manage storage, and handle system operations—all directly within the cloud environment.

---

## 🛠️ Step-by-Step Instructions

### 🔹 Step 1: Launch EC2 Instance

* Go to **AWS Management Console** and search **EC2**.
* The **EC2 Dashboard** will open.
* Go to **Instances** → Click on **Launch Instance**.
* Type server name.
* Select **Amazon Linux AWS**.
* Choose instance type: `t2.micro`.
* Select a key pair.
* In Network Settings, allow **HTTP** and **HTTPS**.
* Click **Launch Instance**.
* Wait until the instance state goes from `Pending` to `Running`.
* Select the instance → click **Connect**.
* Then click **Connect** in the popup.
* Change user:

```bash
sudo su
```

* Update system:

```bash
yum update -y
```

* Install Apache:

```bash
yum install httpd -y
```

* Check Apache status:

```bash
systemctl status httpd
```

* If it's inactive, start it:

```bash
systemctl start httpd
```

* Navigate to web root:

```bash
cd /var/www/html
```

* Create HTML file:

```bash
cat > index.html
# Type content then press Ctrl + D to save
```

---

### 📁 File and Directory Commands

* Create a file:

```bash
cat > file1
# Type something then Ctrl + D
```

* Read a file:

```bash
cat file1
```

* Append to a file:

```bash
cat >> file1
```

* Create multiple files:

```bash
touch file{2..5}
```

* List files:

```bash
ls
```

* List all including hidden:

```bash
ls -a
```

* Long list:

```bash
ll
```

* Long list including hidden:

```bash
ll -a
```

* Delete file:

```bash
rm file2
# Type 'y' when asked
```

* Force delete:

```bash
rm -f file3
```

* Delete folder/files recursively and forcefully:

```bash
rm -rvf file4
```

* Delete all matching pattern:

```bash
rm -rvf file*
```

* Create directory:

```bash
mkdir my
```

* Create subdirectory:

```bash
mkdir my/abc
```

* Navigate:

```bash
cd my/
cd ..
```

* Inside directory create file:

```bash
cat > ql
```

---

### 🔹 File Navigation & Exploration

* Check current location:

```bash
pwd
```

* Navigate to specific folders:

```bash
cd /dev/block
cd ../../bin
```

* List system binaries:

```bash
ls /bin
```

---

### 🔹 User Management

* Add user:

```bash
useradd user1
```

* Switch user:

```bash
su user1
```

---

### 🔹 Step: Using Vim to Edit Files

* Create file:

```bash
touch file1
```

* Write to it:

```bash
cat > file1
```

* Check content:

```bash
cat file1
```

* Edit using Vim:

```bash
vim file1
# Press 'i' to insert
# Press 'Esc' to exit insert mode
# Type ':wq' to write and quit
```

---

### 🔹 Step: File Permissions

* Execution only:

```bash
chmod 111 file1
```

* Write only:

```bash
chmod 222 file1
```

* Read only:

```bash
chmod 444 file1
```

* Full access:

```bash
chmod 777 file1
```

---

### 🔹 Copy/Move Operations

* Copy:

```bash
cp file1 file2
```

* Move:

```bash
mv file1 newname
```
