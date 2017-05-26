# Cisco IOS-XE Ansible playbooks examples

A collection of simple Ansible playbooks to configure a Cisco Catalyst device running IOS-XE

Playbooks have been tested with Ansible 2.3 on a Catalyst 3850 running IOS XE 16.5.1

## Device Credential Management

Device username and password can be set in different ways:
* defining username and password inside the playbook (or in an external file and including the file with the vars_files: directive). 
  NOTE: this way has been deprecated and will be removed in a future version
* defining the ANSIBLE_NET_USERNAME and ANSIBLE_NET_PASSWORD environment variables
* running the playbook with the "-u <user> -k" option and providing the password at run time
