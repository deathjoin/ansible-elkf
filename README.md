# Вторая версия роли в разработке:
https://github.com/deathjoin/ansible-elkf/tree/master/roles/deploy_elkf_v2

# ansible-elfk

Ansible roles to prepare servers and deploy ELKF Stack on Ubuntu.

Tested with Ansible `2.12`

Ansible Vault password: `vault_pass.txt`

## Roles

### prepare_hosts
Install Docker on host with it's dependencies and Python modules for Ansible to manage Docker.

### deploy_elkf
Deploys ELKF Stack on hosts

Default Stack version: `7.7.0`

Tested with: `7.7.0`, `6.7.2`

Config to describe cluster: `elfs-stack.yml`

## Playbooks

Example playbook run:
```bash
ansible-playbook -t deploy -i local_inventory -e "@elkf-stack.yml"  playbooks/install-elkf.yml
```