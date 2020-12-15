# Ansible - Setup an ubuntu Server with Nginx-PHP and host a website

Playbook to install nginx and php to configure a website in an Ubuntu server

##Files

  - nginx-vhost.yaml 
  - hosts
  - vhost_temp.tmpl
  
# nginx-vhost.yaml 
Whole task written in a single Playbook 
### 8 tasks
  -  Upgrade all apt packages
  - Install Nginx and PHP
  - Create website configuration file
  - create soft link for the website
  - Create website folder
  - Upload website contents
  - Unlink the default configuration file
  - Restart nginx service

## hosts
 - lists the hosts with ansible_user and ansible_ssh_private_key_file
 
## vhost_temp.tmpl

Template for vhost configuration file 

## Folder

 - website
Which contains the website files
