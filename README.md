# ansible-elfk

Ansible roles to prepare servers and deploy ELKF Stack on Ubuntu.

Tested with Ansible `2.12`

## Roles

### prepare_hosts
Install Docker on host with it's dependencies and Python modules for Ansible to manage Docker.

### deploy_elkf
Deploys ELKF Stack on hosts

Default Stack version: `7.7.0`

Tested with: `7.7.0`, `6.7.2`