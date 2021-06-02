# Ansible SSH

[![CI](https://github.com/akutschi/ansible_ssh_hardening/actions/workflows/ci.yml/badge.svg)](https://github.com/akutschi/ansible_ssh_hardening/actions/workflows/ci.yml)

This is a very simple role to configure SSH and [fail2ban](https://en.wikipedia.org/wiki/Fail2ban).
Root access is enabled but permitted with key only. 
Password logins are for all users disabled.

> This role does not deploy SSH keys. It is assumed that at least one key is already deployed.

## Requirements

This role does not have any requirements.

## Coverage

Any combination of the following is tested:

- Operating System
  - Ubuntu 20.04 LTS
  - Debian 10
- Ansible
  - 2.9.x
  - 3.x
  - 4.x 
- Python
  - 3.8
  - 3.9

## Install Role

To install this role into your `roles` folder just clone, download or run: 

```bash
ansible-galaxy install --roles-path ./roles git+https://github.com/akutschi/ansible_ssh_hardening.git,v0.2.0
```

## Role Variables

The role itself does not have any settable variables. 

## Dependencies

This role does not have any dependencies.

## Example Playbook

```yml
---
- hosts: servers
  roles:
      - ansible_ssh_hardening
```

# License

GPLv3, see [license](./LICENSE).

# Contributing

Feel free to open issues or merge requests if you find problems or have ideas for improvements. Thank you.
