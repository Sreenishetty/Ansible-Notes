# What is Ansible?
Ansible is a configuration and orchestration management tool where applications are deployed automatically in a variety of environments.

## Step 1 — Installing Ansible
To begin using Ansible as a means of managing your server infrastructure, you need to install the Ansible software on the machine that will serve as the Ansible control node. We’ll use the default Ubuntu repositories for that.

First, refresh your system’s package index with:
$ sudo apt update
$ sudo apt upgrade

Following this update, you can install the Ansible software with:
$ sudo apt -y install software-properties-common
$ sudo apt install software-properties-common
$ sudo apt-add-repository ppa:ansible/ansible
$ sudo apt install ansible

Press Y when prompted to confirm installation.

Your Ansible control node now has all of the software required to administer your hosts. Next, we’ll go over how to set up an inventory file, so that Ansible can communicate with your managed nodes.

# Finding out the ansible Version
Type the following command:
$ ansible --version

## After config the ansible.config file and host file 
Now you can run it as follows:
$ ansible -m ping -all
