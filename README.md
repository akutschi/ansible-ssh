# Ansible SSH

[![Molecule](https://github.com/akutschi/ansible_ssh/actions/workflows/ci.yml/badge.svg)](https://github.com/akutschi/ansible_ssh/actions/workflows/ci.yml)

This is a very simple role to configure SSH. 
Root access is enabled but permitted with key only. 
Password logins are for all users disabled.

> This role does not deploy SSH keys. It is assumed that keys are already deployed.

## Requirements

This role does not have any requirements.

## Coverage

Any combination of the following is tested:

- Operating System
  - Ubuntu 20.04 LTS or
  - Debian 10
- Ansible
  - 2.9.x or
  - 3.x or
  - 4.x 
- Python
  - 3.8 or
  - 3.9

## Role Variables

There are no settable variables in this role.

## Dependencies

This role does not have any dependencies.

## Example Playbook

The setup is quite simple.
Just clone or download this role into your `roles` folder and set up the playbook similar to this example:

```yml
---
- hosts: servers
  roles:
      - ansible_ssh
```

# License

GPLv3, see [license](./LICENSE).

# Contributing

Feel free to open issues or merge requests if you find problems or have ideas for improvements. Thank you.
