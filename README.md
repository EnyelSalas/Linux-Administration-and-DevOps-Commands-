# Linux & DevOps Command Cheat Sheet

Welcome to the **Linux & DevOps Command Cheat Sheet**! This repository provides a categorized collection of essential commands for Linux system administration and DevOps tasks. It is designed for **educational purposes**, helping users quickly access and learn the commands they need for daily tasks, certifications, or professional development.

---

## Table of Contents
1. [User Management](#user-management)
2. [File and Directory Management](#file-and-directory-management)
3. [Permissions & Ownership](#permissions--ownership)
4. [Process Management](#process-management)
5. [Networking](#networking)
6. [Package Management](#package-management)
7. [Cron Jobs & Scheduled Tasks](#cron-jobs--scheduled-tasks)
8. [System Monitoring](#system-monitoring)
9. [Docker Commands](#docker-commands)
10. [Git Commands](#git-commands)
11. [Miscellaneous](#miscellaneous)
12. [Advanced Networking Protocol Commands](#advanced-networking-protocol-commands)
13. [Configuration Management Tools](#configuration-management-tools)

---

## User Management
- **Add a user**: `sudo useradd <username>`
- **Delete a user**: `sudo userdel <username>`
- **Change user password**: `passwd <username>`
- **List logged-in users**: `who` or `w`
- **Switch user**: `su - <username>`
- **Check user information**: `id <username>`
- **Lock a user account**: `sudo usermod -L <username>`
- **Unlock a user account**: `sudo usermod -U <username>`

---

## File and Directory Management
- **List directory contents**: `ls -la`
- **Change directory**: `cd <directory>`
- **Copy files**: `cp <source> <destination>`
- **Move files**: `mv <source> <destination>`
- **Remove files**: `rm <file>`
- **Remove directories**: `rm -r <directory>`
- **Create a directory**: `mkdir <directory>`
- **View file contents**: `cat <file>` or `less <file>`
- **Search inside files**: `grep '<text>' <file>`

---

## Permissions & Ownership
- **Change file permissions**: `chmod <mode> <file>`
- **Change ownership**: `chown <owner>:<group> <file>`
- **Check permissions**: `ls -l`
- **Recursive permission change**: `chmod -R <mode> <directory>`
- **Recursive ownership change**: `chown -R <owner>:<group> <directory>`

---

## Process Management
- **List all processes**: `ps aux`
- **Kill a process**: `kill <PID>`
- **Force kill**: `kill -9 <PID>`
- **Find a process by name**: `pgrep <name>`
- **System resource usage**: `top` or `htop`
- **Start a background process**: `<command> &`
- **Bring process to foreground**: `fg <job_id>`

---

## Networking
- **Check IP address**: `ip a` or `ifconfig`
- **Ping a host**: `ping <host>`
- **Display routing table**: `route` or `ip route`
- **Test DNS resolution**: `nslookup <domain>` or `dig <domain>`
- **Check open ports**: `netstat -tuln` or `ss -tuln`
- **Traceroute**: `traceroute <host>`

---

## Package Management
### Ubuntu/Debian
- **Update package list**: `sudo apt update`
- **Upgrade packages**: `sudo apt upgrade`
- **Install package**: `sudo apt install <package>`
- **Remove package**: `sudo apt remove <package>`

### Red Hat/CentOS
- **Install package**: `sudo yum install <package>`
- **Remove package**: `sudo yum remove <package>`
- **List installed packages**: `sudo yum list installed`

---

## Cron Jobs & Scheduled Tasks
- **Edit cron jobs**: `crontab -e`
- **List cron jobs**: `crontab -l`
- **Cron syntax**: `<minute> <hour> <day> <month> <day_of_week> <command>`
  - Example: `0 3 * * 1 /path/to/script.sh` (Run script every Monday at 3:00 AM)

---

## System Monitoring
- **Disk usage**: `df -h`
- **Directory size**: `du -sh <directory>`
- **Memory usage**: `free -m`
- **CPU info**: `lscpu`
- **System uptime**: `uptime`

---

## Docker Commands
- **List running containers**: `docker ps`
- **List all containers**: `docker ps -a`
- **Start a container**: `docker start <container>`
- **Stop a container**: `docker stop <container>`
- **Remove a container**: `docker rm <container>`
- **Build an image**: `docker build -t <image_name> .`
- **Run a container**: `docker run -d <image>`

---

## Git Commands
- **Clone a repository**: `git clone <repo_url>`
- **Check status**: `git status`
- **Stage changes**: `git add <file>`
- **Commit changes**: `git commit -m "<message>"`
- **Push changes**: `git push origin <branch>`
- **Pull updates**: `git pull origin <branch>`
- **Check log**: `git log`

---

## Advanced Networking Protocol Commands
- **Check DNS records**: `dig <domain> ANY`
- **SSL Certificate Information**: `openssl s_client -connect <domain>:443`
- **FTP connection**: `ftp <host>`
- **SCP file transfer**: `scp <file> <user>@<host>:<path>`
- **View active connections**: `lsof -i`

---

## Configuration Management Tools
### Ansible
- **Run playbook**: `ansible-playbook <playbook.yml>`
- **Ping nodes**: `ansible all -m ping`

### Terraform
- **Initialize**: `terraform init`
- **Apply changes**: `terraform apply`
- **Destroy infrastructure**: `terraform destroy`

---

## Contributions
This cheat sheet is a work in progress. Contributions are welcome! Feel free to submit issues or pull requests to improve this resource.
