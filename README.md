# README.md - ansible-role-control-machine

This playbook will finish setting up the local machine as the Ansible control
machine.

It requires elevated privileges and should be run with the `--ask-become-pass` 
or `-K` flag.

Example:

```bash
ANSIBLE_CONFIG=ansible.cfg ansible-playbook ./roles/ansible-role-control-machine/example-playbook.yaml -i localhost

# or

ANSIBLE_ROLES_PATH=./roles ansible-playbook ./roles/ansible-role-control-machine/example-playbook.yaml -i localhost
```
