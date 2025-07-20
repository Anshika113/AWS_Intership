**Linux Commands**

**Introduction:**

In AWS, especially when working with EC2 Linux instances, Linux commands are essential for managing and interacting with the virtual server environment. After connecting to a Linux instance via SSH, users use Linux commands to perform tasks like:

- Navigating directories (cd, ls)
- Managing files (cp, mv, rm, nano, vim)
- Installing software (yum, apt-get)
- Monitoring system performance (top, htop, df, free)
- Managing permissions and users (chmod, chown, adduser)
- Starting and stopping services (systemctl, service)
- Transferring files (scp, rsync)
- Running scripts and automating tasks (bash, cron)

These commands enable users to configure servers, deploy applications, manage storage, and handle system operations—all directly within the cloud environment.

**Step by Step Instructions:**

**Step 1:**

- Go to “AWS Management Console” and search “EC2”.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.001.png)              ![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.002.png)

- The “EC2 Dashboard” will open.
- Go to “Instance”.
- Click on “Launch Instance”.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.003.png)

- Type Server name.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.004.png)

- Select “Amazon Linux aws”.  

  ![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.005.png)

- Select “t2.micro” instance type.
- Select key pair.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.006.png)

- In Network Setting, Allow https and https.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.007.png)

- Click on “Launch Instance”.
- ![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.008.png)
- Wait until the instance state goes from “Pending” to “Running”.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.009.png)

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.010.png)

- Now, Select the server and then click on “Connect”.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.011.png)

- Then click on connect.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.012.png)

- Change user with the help of “sudo su” command.
- Then for check update type “yum update -y”.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.013.png)

- For installation type “yum install httpd -y”

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.014.png)

- Whether package is start or stop you have to type command “systemctl status httpd”.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.015.png)

- It shows that “inactive(dead)”.
- For Starting package, type “systemctl start httpd”.

`      `![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.016.png)

- For html, type command “cd /var/www/html”.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.017.png)

- For typing the text, type “cat >index.html” and then type the message, after this press “Ctrl+ D” for exit.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.018.png)

- For Creating file, “cat file1” or “cat > file1” and type something after this type “Ctrl+ D”.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.019.png)

- For read, type “cat file1” command.

`            `![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.020.png)

- For edit more line type “cat >> file1” command.

`          `![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.021.png) 

- For creating multiples files, type “touch file{2..5}” command.
- For check file, type “ls” command.

  `   `![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.022.png)

- For hidden file or dot file, type “ls-a” command. It stand for list all.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.023.png)

- For long list, type “ll” command.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.024.png)

- In long list, for check hidden or dot file type “ll -a” command.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.025.png)

- For remove file, type “rm file2” command. It asks permission “remove regular empty file ‘file2’?” type “y”.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.026.png)

- If you don’t want permission to remove file type “rm -f file3” command. f stands for forcefully.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.027.png)

- For deleting internal files, type “rm -rvf file4” command. rvf stands for “recursive verbose forcefully” and it shows “removed”.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.028.png)

- For removing all files with the name of ‘file’, type “rm -rvf file\*”.

  ![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.029.png)

- For creating directory, type “mkdir my” command and then “my” name directory created.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.030.png)

- For creating internal file in “my” type “mkdir my/abc” command.![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.031.png)

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.032.png)

- For go to internal file of my, type “cd my/” command.

`               `![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.033.png)

- For typing internal file type “cat > ql” command where ql is file.

  ![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.034.png)

- For going one step back, type “cd ..” command.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.035.png)

- Type “ll -a” command where you see those files which start from ‘d’ means ‘directory’ and ‘l’ means ‘list’ and ‘-‘ means ‘file’.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.036.png)

- For going to ‘block’, type “cd /dev/block” command.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.037.png)

- For going to ‘bin’, type “cd ../../bin”.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.038.png)

- If you forget your current location, type “pwd” command.

`          `![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.039.png)

- For check list in, type “ls /bin” command.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.040.png)

- For adding user, type “useradd user1” command where ‘user1’ is user name.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.041.png)

- For switching user, type “su user1” command.

`             `![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.042.png)

- **For update using vim:**
- Create file type “touch file1” command.
- For typing, type “cat >file1” command.
- For check, type “cat file1” command.
- For update, type “vim file1” command.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.043.png)

- For insert, type ‘i’ from keyboard.

`     `![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.044.png)

- For exit, click on ‘esc’ from keyboard.
- For save, type ‘:’.
- For write, type ‘w’ from keyboard.
- For quit, type ‘q’ from keyboard.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.045.png)![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.046.png)![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.047.png)![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.048.png)![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.049.png)![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.050.png)![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.051.png)![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.052.png)

- Then see updated version.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.053.png)




**For changing file permission:**

- Only execution permission, type “chmod 111 file1” command. ‘x’ stands for ‘execute’.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.054.png)

- Only write permission, type “chmod 222 file1” command. ‘w’ stands for ‘write’.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.055.png)![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.056.png)

- Only read permission, type “chmod 444 file1” command. ‘r’ stands for ‘read’.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.057.png)![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.058.png)               ![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.059.png)

- Only all permission, type “chmod 777 file1” command. ‘rwx’ stands for ‘read write execution’.

![](Aspose.Words.c8969eb7-cbe8-4521-8396-103420fa857f.060.png)

- For copy, type file name with “cp”.
- For move, type file name with “mv”.
