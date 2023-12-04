# Born2beRoot

## Introduction

This document outlines a System Administration exercise, Born2beRoot, which introduces participants to the world of virtualization. The project involves setting up a server with specific rules, focusing on minimal services and strong security measures.

## General Guidelines

- The use of VirtualBox (or UTM if unable to use VirtualBox) is mandatory.
- Submission requires a `signature.txt` file at the root of the repository, containing the signature of the machine's virtual disk.

## Mandatory Part

### Server Setup Rules

- Operating System: Latest stable version of Debian or Rocky (no testing/unstable).
- Forbidden: Installation of X.org or any equivalent graphics server.
- SELinux must be running at startup for Rocky, and AppArmor for Debian.
- At least 2 encrypted partitions using LVM.
- SSH service running on port 4242 only, disallowing root login.
- Firewall setup using UFW (or firewalld for Rocky) to allow only port 4242.
- Hostname: Your login ending with 42 (e.g., wil42).
- Strong password policy for all users.
- Installation and configuration of sudo following strict rules.

### Monitoring Script (monitoring.sh)

- Displays system information on all terminals every 10 minutes.
- Information includes architecture, processor details, memory usage, disk usage, CPU load, last boot time, LVM usage, active connections, users, IP address, and more.

## Bonus Part

- Bonus tasks include setting up partitions, a WordPress website, and an additional service of choice.
- Adapt UFW/Firewalld rules for bonus services.

## Notes

### What I Learned

- **Virtualization Basics:** Learned about setting up virtual machines using VirtualBox or UTM.
- **System Administration Skills:** Gained hands-on experience in configuring and securing a server.
- **Security Measures:** Implemented strong password policies, SSH restrictions, and firewall configurations.
- **Monitoring Scripts:** Developed a bash script for monitoring system information.
- **Troubleshooting:** Acquired skills in debugging and solving configuration issues.
- **Understanding SELinux and AppArmor:** Learned about mandatory access controls and security modules.
- **Documentation:** Improved documentation skills by creating a clear and structured README.
