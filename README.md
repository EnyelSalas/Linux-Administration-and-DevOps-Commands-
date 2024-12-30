# Linux-Administration-and-DevOps-Commands-
Linux &amp; DevOps Command Cheat Sheet This repository serves as a comprehensive and categorized reference for Linux administration and DevOps commands. It is designed for educational purposes, aimed at helping beginners and professionals Linux system administration, DevOps practices, networking protocols, and command-line.

1. User Management

Add a user: sudo useradd <username>

Delete a user: sudo userdel <username>

Change user password: passwd <username>

List logged-in users: who or w

Switch user: su - <username>

Check user information: id <username>

Lock a user account: sudo usermod -L <username>

Unlock a user account: sudo usermod -U <username>

2. File and Directory Management

List directory contents: ls -la

Change directory: cd <directory>

Copy files: cp <source> <destination>

Move files: mv <source> <destination>

Remove files: rm <file>

Remove directories: rm -r <directory>

Create a directory: mkdir <directory>

View file contents: cat <file> or less <file>

Search inside files: grep '<text>' <file>

3. Permissions & Ownership

Change file permissions: chmod <mode> <file>

Change ownership: chown <owner>:<group> <file>

Check permissions: ls -l

Recursive permission change: chmod -R <mode> <directory>

Recursive ownership change: chown -R <owner>:<group> <directory>

4. Process Management

List all processes: ps aux

Kill a process: kill <PID>

Force kill: kill -9 <PID>

Find a process by name: pgrep <name>

System resource usage: top or htop

Start a background process: <command> &

Bring process to foreground: fg <job_id>

5. Networking

Check IP address: ip a or ifconfig

Ping a host: ping <host>

Display routing table: route or ip route

Test DNS resolution: nslookup <domain> or dig <domain>

Check open ports: netstat -tuln or ss -tuln

Traceroute: traceroute <host>

6. Package Management

Ubuntu/Debian:

Update package list: sudo apt update

Upgrade packages: sudo apt upgrade

Install package: sudo apt install <package>

Remove package: sudo apt remove <package>

Red Hat/CentOS:

Install package: sudo yum install <package>

Remove package: sudo yum remove <package>

List installed packages: sudo yum list installed

7. Cron Jobs & Scheduled Tasks

Edit cron jobs: crontab -e

List cron jobs: crontab -l

Cron syntax: <minute> <hour> <day> <month> <day_of_week> <command>

Example: 0 3 * * 1 /path/to/script.sh (Run script every Monday at 3:00 AM)

8. System Monitoring

Disk usage: df -h

Directory size: du -sh <directory>

Memory usage: free -m

CPU info: lscpu

System uptime: uptime

11. Miscellaneous

Check system logs: tail -f /var/log/syslog

Reboot system: sudo reboot

Shutdown system: sudo shutdown -h now

Set system hostname: sudo hostnamectl set-hostname <hostname>

Test connection: curl <url>

12. Advanced Networking Protocol Commands

Check DNS records: dig <domain> ANY

SSL Certificate Information: openssl s_client -connect <domain>:443

FTP connection: ftp <host>

SCP file transfer: scp <file> <user>@<host>:<path>

View active connections: lsof -i
