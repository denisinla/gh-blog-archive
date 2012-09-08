---
layout: post
title: Dropbox on Fedora 17
tags: dropbox - fedora17
---

![Fedora 17](http://media.tumblr.com/tumblr_m9mc8qC4TY1qz7r46.jpg)

**Configure Dropbox Repository**  
Create a file called dropbox.repo inside of ``/etc/yum.repos.d``  

``$ cd /etc/yum.repos.d``  
``$ sudo vim dropbox.repo``
  
Paste the following:  

``[Dropbox]
name=Dropbox Repository
baseurl=http://linux.dropbox.com/fedora/17/
gpgkey=http://linux.dropbox.com/fedora/rpm-public-key.asc``  

Once you have the repo file saved to yum we want to enable the repository:  

``$ sudo yum-config-manager --enable``   

This will enable all installed repositories.

**Installing Dropbox**  
Run yum install using the command: 

``$sudo yum install nautilus-dropbox --nogpgcheck``  

Notice how ``--nogpgcheck`` parameter was added, since the rpm public key seems to return a 404 on Dropbox.

**Completing the Installation**   
After installation is done, you need to run Dropbox (Applications >> Internet >> Dropbox) application to complete the installation and configure an user account.