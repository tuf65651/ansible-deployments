# Deploy Web App
This Ansible Role can be used to deploy TheWimbo Web Interface. It clones the correct git repo, pip installs packages and calls deploy function.

## Typical use
Include this role in an ansible playbook.

**Requirements:**
Hosts must have connectivity to package manager repositories.
Deployment scripts rely on specific environment variables and *will* crash if they aren't set.
Ansible `environment`  option can be used to set environment variables within the context of a playbook's execution.