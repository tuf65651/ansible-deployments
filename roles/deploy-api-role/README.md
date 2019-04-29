# Deploy API
This Ansible Role can be used to deploy TheWimbo REST API. It clones the correct git repo, pip installs packages and calls deploy function.

## Typical use
Include this role in an ansible playbook.

**Requirements:**
Hosts must have connectivity to package manager repositories.
Deployment scripts rely on specific environment variables and *will* crash if they aren't set.
Ansible `environment`  option can be used to set environment variables within the context of a playbook's execution.
Connections to specific database and file storage instances are hardcoded. If these are unavailable, API will not run.

_Notes: for formal API Specs, see documentation in REST_API repo_