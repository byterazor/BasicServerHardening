# Basic Hardening Ansible Script

## Maintainer 

- Dominik Meyer <dmeyer@federationhq.de>

## Description

Some basic Security Hardening plays using Ansible

### Hardening Features

- create an issue and issue.net from the provided template
- disable root login for ssh
- set maximum number of concurrent alive ssh client sessions
- set maximum number of SSH sessions
- set ssh compression to delayed
- set ssh maximum number of authentication retries 
- disable ssh TCP keep alive
- disable X11 forwarding
- enable SSH banner
- default umask in login.defs
- setup minimum password age in login.defs
- setup maximum password age in login.defs
- enable spoof protection
- enable syn cookies
- disable ICMP redirects
- enable kernel address space layout randomization (ASLR)
- install and enable fail2ban
- install and enable rkhunter
- install per user temp dirs
- install debsums for verifying package integrity
- install the debsecan tool
- install lynis
- install usbguard
- disable core dumps
- disable setuid applications core dumps
- disable kernel kernel core dumps
- set pam maxlogins
- set pam nproc
- Disallow opening files in world writeable sticky directories
- Disallow opening fifos in world writeable sticky directories
- Protect hardlinks
- Protect symlinks
- Disallow bpf loading for normal users
- harden bpf jit compilter

# Usage

Clone this repository into the roles folder of your playbook and 
add the role  

Available variables used in your host repository can be found in defaults/main.yml.

# LICENSE

GPLv3