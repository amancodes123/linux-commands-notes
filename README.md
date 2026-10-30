# 🐧 Linux Commands Notes for Cloud & DevOps

Welcome to my Linux Commands Revision Repository!

I'm revising and documenting the Linux commands I have learned as part of my Cloud Computing and DevOps journey.

After working on AWS projects and learning Git & GitHub, I'm strengthening my Linux fundamentals through regular revision and hands-on practice.

The goal of this repository is to maintain organized, practical notes that I can refer to during projects, troubleshooting, and interview preparation.

---

## 🎯 Objectives

- Revise essential Linux commands.
- Strengthen command-line fundamentals.
- Practice file and directory management.
- Understand Linux permissions and ownership.
- Learn user and process management.
- Practice networking and troubleshooting commands.
- Understand log analysis and system monitoring.
- Build a foundation for Bash scripting and DevOps automation.
- Maintain quick-reference notes for interviews.

---

## 📚 Topics Covered

| No. | Topic | Description |
|---|---|---|
| 01 | File & Directory Management | Create, list, copy, move, and delete files and directories |
| 02 | File Content & Searching | Read files, search text, and locate files |
| 03 | Permissions & Ownership | Manage file permissions and ownership |
| 04 | Users & Groups | Create users and manage groups |
| 05 | Process Management | Monitor and manage running processes |
| 06 | System Monitoring | Check memory, disk usage, and system uptime |
| 07 | Networking Commands | Check connectivity and troubleshoot networks |
| 08 | Log Analysis | Read, filter, and monitor system logs |
| 09 | Package Management | Install, update, and remove software packages |
| 10 | Services & systemd | Manage Linux services |
| 11 | SSH & SCP | Connect to remote servers and transfer files |
| 12 | Archives & Compression | Create and extract compressed archives |
| 13 | Disk Management | Explore disks, filesystems, and storage |
| 14 | Environment Variables | Understand and manage environment variables |
| 15 | Bash Scripting Basics | Automate repetitive tasks using shell scripts |
| 16 | Linux Shortcuts | Improve command-line productivity |

---

## 🛠️ Essential Linux Commands

### 1. File and Directory Management

```bash
pwd                 # Display current working directory
ls                  # List files and directories
ls -la              # List all files with detailed information
cd /path/to/dir     # Change directory
mkdir project       # Create a directory
touch file.txt      # Create an empty file
cp file.txt copy.txt # Copy a file
mv file.txt new.txt # Move or rename a file
rm file.txt         # Delete a file
rmdir empty_dir     # Remove an empty directory
```

### 2. File Content and Searching

```bash
cat file.txt                    # Display file contents
less file.txt                   # Read a file page by page
head -n 10 file.txt             # Display the first 10 lines
tail -n 10 file.txt             # Display the last 10 lines
tail -f application.log         # Follow new log entries
grep "error" application.log    # Search for a word
grep -i "error" application.log # Search without case sensitivity
find /var/log -name "*.log"     # Find log files
wc -l file.txt                  # Count lines
```

### 3. Permissions and Ownership

```bash
ls -l file.txt                  # Check file permissions
chmod 644 file.txt              # Set file permissions
chmod +x script.sh              # Make a script executable
chown user:user file.txt        # Change owner and group
chgrp developers file.txt       # Change group ownership
```

### 4. Users and Groups

```bash
whoami                 # Display current user
id                     # Display user and group IDs
who                    # Show logged-in users
groups                 # Display current user's groups
sudo useradd devuser   # Create a user on supported systems
sudo passwd devuser    # Set or change a user's password
```

### 5. Process Management

```bash
ps aux                 # Display running processes
top                    # Monitor processes in real time
pgrep nginx            # Find process IDs by name
kill PID               # Send a termination signal to a process
jobs                   # Display jobs in the current shell
```

### 6. System Monitoring

```bash
df -h                  # Check filesystem disk usage
du -sh directory/      # Check directory size
free -h                # Display memory usage
uptime                 # Show system uptime and load averages
uname -a               # Display system information
```

### 7. Networking Commands

```bash
ip addr                # Display network interfaces and IP addresses
ip route               # Display routing table
ping -c 4 example.com  # Test connectivity
curl -I https://example.com  # Check HTTP response headers
ss -tuln               # Display listening TCP/UDP sockets
```

### 8. Log Analysis

```bash
tail -f /var/log/syslog
grep -i "error" application.log
grep -n "failed" application.log
awk '{print $1}' access.log
```

**Note:** Log file locations vary by Linux distribution and application. For example, some systems use `/var/log/messages` instead of `/var/log/syslog`.

### 9. Package Management

```bash
sudo apt update              # Update package lists on Debian/Ubuntu
sudo apt upgrade             # Upgrade installed packages
sudo dnf install nginx       # Install a package on supported DNF systems
sudo yum install git         # Install a package on supported YUM systems
```

### 10. Services and systemd

```bash
sudo systemctl status nginx   # Check service status
sudo systemctl start nginx    # Start a service
sudo systemctl stop nginx     # Stop a service
sudo systemctl restart nginx  # Restart a service
sudo systemctl enable nginx   # Enable a service at startup
```

### 11. SSH and SCP

```bash
ssh user@server-ip
scp file.txt user@server-ip:/home/user/
scp user@server-ip:/home/user/file.txt .
```

**Note:** Use the correct username, server address, SSH key, and destination path for your environment.

### 12. Archives and Compression

```bash
tar -cvf archive.tar directory/
tar -xvf archive.tar
tar -czvf archive.tar.gz directory/
tar -xzvf archive.tar.gz
```

---

## 💻 Hands-On Practice

I practice Linux commands using a Linux environment and apply them to practical scenarios.

Examples include:

- Navigating directories and managing files.
- Creating users and configuring permissions.
- Monitoring processes and system resources.
- Searching application logs for errors.
- Connecting to remote Linux servers using SSH.
- Transferring files between systems using SCP.
- Managing services such as Nginx.
- Troubleshooting connectivity and application issues.
- Preparing for Bash scripting and automation.

---

## ☁️ Connection to Cloud & DevOps

Linux is an important part of my Cloud and DevOps learning journey.

I use these fundamentals to build a stronger understanding of:

- AWS EC2 and Linux server administration.
- Remote server access using SSH.
- Web server setup and management.
- Application log monitoring.
- Troubleshooting cloud-hosted applications.
- Automation using Bash scripts.
- Infrastructure and deployment workflows.

---

## 📈 Learning Approach

My approach is simple:

1. Revise the command.
2. Understand its purpose and options.
3. Practice it in a Linux environment.
4. Apply it to a practical scenario.
5. Document the command with examples.
6. Revisit it regularly.

This repository will continue to evolve as I revise and practice more Linux commands.

---



## ⭐ Support

If you find these notes useful, consider starring this repository.

Thanks for visiting! 🚀

**Learning in public | Practicing consistently | Growing in Cloud & DevOps**
