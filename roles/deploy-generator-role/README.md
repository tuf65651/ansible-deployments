# Set Up Neural Net
This Ansible Role can be used to deploy TheWimbo Web Neural Net. It clones the correct git repo, pip installs packages and calls a song generate to verify setup. Unlike other roles in this project, this role doesn't start a background process. It just sets up Neural Net.

## Typical use
Include this role in an ansible playbook.

**Requirements:**
Hosts must have connectivity to package manager repositories.
Deployment scripts rely on specific environment variables and may crash if they aren't set.
Ansible `environment`  option can be used to set environment variables within the context of a playbook's execution.

_Note: For Documentation on Neural Net, including samples of training and song generation, see Neural Net repo_