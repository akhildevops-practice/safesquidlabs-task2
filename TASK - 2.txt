TASK - 2
Script for Automating Security Audits and Server Hardening on

Prerequisite: 
- Create an Ubuntu EC2 Instance to create the Script for Automating Security Audits and Server Hardening on.

Process:
- Login into an instance using ssh and git bash.

* ssh -i "ansible-prac.pem" ubuntu@ec2-3-110-30-110.ap-south-1.compute.amazonaws.com

- After login update the packages.

* sudo apt update

- Create a file named as security-audit-task.sh, sh is an file extension used in bash to execute the script and change the access permission of files and directories, give executable permissions for the script.

* touch security-audit-task.sh
* chmod +x security-audit-task.sh
* Write the Script and execute it.
* ./security-audit-task.sh

# users and user-related issues:
./security-audit-task.sh --users

# file and directory permissions:
./security-audit-task.sh --permissions

# running services:
./security-audit-task.sh --services

# firewall status and open ports:
./security-audit-task.sh --firewall

# network settings:
./security-audit-task.sh --network

# security updates:
./security-audit-task.sh --updates

#  SSH configuration:
./security-audit-task.sh --ssh

# Check and disable IPv6:
./security-audit-task.sh --ipv6

# GRUB bootloader security:
./security-audit-task.sh --bootloader

# logs for suspicious activity:
./security-audit-task.sh --logs

#Run the script with an interval to refresh data every few seconds:

./security-audit-task.sh --users --permissions --interval 10


