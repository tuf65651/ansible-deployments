# Ansible Deployments
This folder contains ansible roles and overhead files for automating deployment of TheWimbo Application
Roles contain their own README files.

## Typical use
In this project root directory, write an ansible playbook that calls the other roles.
An example of such a playbook ```provision.yml``` has been included in this directory.
Target machines should be included in the inventory file mentioned by the ansible.cfg file, by IP Address or FQDN.
IP addresses should not be placed in code.

## Check setup
```verify_ansible_connection.yml``` is a playbook that verifies ansible install and connectivity to targets.
It just connects, discovers host facts, and prints out hostname.

**Requirements**
`provision.yml` sets environment using vaulted secrets. Deployments in this project rely on environment variables.
These variables must be set, either in the host system, or using ansible's `environment` keyword. If you are confident in the security of your connection, and in the security of the system running engine, you can set these variables in plain text, using the `environment` keyword.