# SOP for Common Ubuntu Commands

## Author Information

| Created by      | Created on         | Version          | Last updated ON   | pre Reviewer       | L0 Reviewer     | L1 Reviewer          |    L2 Reviewer    |
|-----------------|--------------------|------------------|-------------------|--------------------|-----------------|----------------------|-------------------|
| Abhishek saini  |  16-07-2025        | V 1.0            |     18-07-2025    |  Prashant          | -    |      -  |   - |

---
## Table of Contents   
- [Objective](#objective)
- [System Information](#system-information)    
- [User Management](#user-management)                  
- [Directory & File Operations](#directory--file-operations) 
- [Permission & Ownership](#permission--ownership)     
- [Networking](#networking)                            
- [Reboot and Shutdown](#reboot-and-shutdown)          
- [File Viewing & Editing](#file-viewing--editing)    



## Objective
- To provide a detailed list of frequently used Ubuntu commands with their descriptions and best practices. This SOP helps the users to perform basic system tasks effectively on Ubuntu systems.

---

## System Information

### Description:
- Commands to get kernel, hostname, memory, disk usage, and uptime information.

### Commands:
```bash
uname -a         # Show system information including kernel version
```
```bash
hostnamectl       # Display hostname, OS, kernel, architecture, etc.
```
```bash
df -h             # Show disk space usage in human-readable format
```
```bash
free -h           # Show memory usage in human-readable format
```
```bash
uptime            # Show how long the system has been running and load average
```
---

## User Management

### Description:
- Manage user accounts and groups.

### Commands:
```bash
sudo adduser <username>               # Add a new user interactively
```
```bash
sudo userdel <username>               # Delete an existing user
```
```bash
sudo usermod -aG <group> <username>   # Add user to a supplementary group
```
```bash
id <username>                         # Display UID, GID, and groups of the user
```
---

## Directory & File Operations

### Description:
- Create, view, move, delete, and manage files and directories.

### Commands:
```bash
ls -l                         # List files and directories with details
```
```bash
cd /path/to/dir               # Change current directory
```
```bash
mkdir new_folder              # Create a new directory
```
```bash
rm -rf folder/                # Remove a directory and its contents recursively
```
```bash
touch file.txt                # Create a new empty file
```
```bash
cat file.txt                  # Display contents of a file
```
```bash
cp source.txt dest.txt        # Copy file from source to destination
```
```bash
mv oldname.txt newname.txt    # Rename or move a file
```
---

## Permission & Ownership

### Description:
- Modify file permissions and ownership.

### Commands:
```bash
chmod +x script.sh            # Add execute permission to a script
```
```bash
chmod 755 file                # Set permission: rwxr-xr-x
```
```bash
chown user:group file         # Change file owner and group
```
---

## Networking

### Description:
- View IP configuration, test connectivity, and check network services.

### Commands:
```bash
ip a                          # Display all IP addresses and network interfaces
```
```bash
ping <hostname>               # Check connectivity to a remote host
```
```bash
netstat -tuln                 # Show active listening ports (TCP/UDP)
```
```bash
curl http://localhost:3000    # Send HTTP request to test a local service
```
---

## Reboot and Shutdown

### Description:
- Restart or shut down the machine.

### Commands:
```bash
sudo reboot                   # Reboot the system
```
```bash
sudo shutdown now             # Shut down the system immediately
```
---

## File Viewing & Editing

### Description:
- Read or modify file content using terminal editors.

### Commands:
```bash
cat file.txt                  # Display file content in terminal
```
```bash
less file.txt                 # View file one page at a time
```
```bash
nano file.txt                 # Edit file using nano (beginner friendly)
```
```bash
vim file.txt                  # Edit file using vim (advanced editor)
```
---
## Contact Information

| **Name**           | **Email address**                         |
|--------------------|--------------------------------------------|
| Abhishek saini    | [abhishek.saini.snaatak@mygurukulam.co |

---

## References

| **Link**                                                                 | **Description**                                   |
|--------------------------------------------------------------------------|---------------------------------------------------|
| [Linux common commands– ](https://www.digitalocean.com/community/tutorials/linux-commands) | Document format followed from this link.          |
