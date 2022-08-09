# What is Ansible?
Ansible is a radically simple IT automation system. It handles configuration management, application deployment, cloud provisioning, ad-hoc task execution, network automation, and multi-node orchestration. Ansible makes complex changes like zero-downtime rolling updates with load balancers easy.

## Design Principles
    Have an extremely simple setup process with a minimal learning curve.
    Manage machines quickly and in parallel.
    Avoid custom-agents and additional open ports, be agentless by leveraging the existing SSH daemon.
    Describe infrastructure in a language that is both machine and human friendly.
    Focus on security and easy auditability/review/rewriting of content.
    Manage new remote machines instantly, without bootstrapping any software.
    Allow module development in any dynamic language, not just Python.
    Be usable as non-root.
    Be the easiest IT automation system to use, ever.

## Step 1 — Installing Ansible
To begin using Ansible as a means of managing your server infrastructure, you need to install the Ansible software on the machine that will serve as the Ansible control node. We’ll use the default Ubuntu repositories for that.

## First, refresh your system’s package index with:
$ sudo apt update
$ sudo apt upgrade

## Following this update, you can install the Ansible software with:
```
$ sudo apt -y install software-properties-common
$ sudo apt install software-properties-common
$ sudo apt-add-repository ppa:ansible/ansible
$ sudo apt install ansible
```

Press Y when prompted to confirm installation.

Your Ansible control node now has all of the software required to administer your hosts. Next, we’ll go over how to set up an inventory file, so that Ansible can communicate with your managed nodes.

## Finding out the ansible Version
Type the following command:
$ ansible --version

## After config the ansible.config file and host file 
Now you can run it as follows:
$ ansible -m ping -all
