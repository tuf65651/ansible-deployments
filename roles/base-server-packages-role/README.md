# Base Server Packages
This Ansible Role is designed to smooth assumptions about server OS. Run it before attempting deployment on a fresh linux machine.
This role has only been tested with apt managed machines. Use yum at your own risk.

## Typical use
Include this role in an ansible playbook.

**Requirements:**
Hosts must have connectivity to package manager repositories.