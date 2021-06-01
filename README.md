# Ansible SSH

[![CI](https://github.com/akutschi/ansible_ssh_hardening/actions/workflows/ci.yml/badge.svg)](https://github.com/akutschi/ansible_ssh_hardening/actions/workflows/ci.yml)

This is a very simple role to configure SSH and [fail2ban](https://en.wikipedia.org/wiki/Fail2ban).
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

The role itself does not have any settable variables. 
But the dependency has variables.
Check the [README](https://github.com/akutschi/ansible_ufw) of Ansible UFW for the role variables.

## Dependencies

This role depends on [Ansible UFW](https://github.com/akutschi/ansible_ufw) and will be installed as dependency. 

## Example Playbook

The setup is quite simple.
Just clone or download this role into your `roles` folder and set up the playbook similar to this example:

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
