Upgrade Packages ansible role
=========

[![CI](https://github.com/dtoch56/ansible-role-upgrade-packages/workflows/CI/badge.svg?event=push)](https://github.com/dtoch56/ansible-role-upgrade-packages/actions?query=workflow%3ACI)
[![Release](https://github.com/dtoch56/ansible-role-upgrade-packages/workflows/Release/badge.svg?event=push)](https://github.com/dtoch56/ansible-role-upgrade-packages/actions?query=workflow%3ARelease)
[![Role](https://img.shields.io/ansible/role/55436)](https://galaxy.ansible.com/dtoch56/upgrade_packages)
[![Downloads](https://img.shields.io/badge/dynamic/json?color=blueviolet&label=Galaxy%20Downloads&query=%24.download_count&url=https%3A%2F%2Fgalaxy.ansible.com%2Fapi%2Fv1%2Froles%2F55436%2F%3Fformat%3Djson)](https://galaxy.ansible.com/dtoch56/upgrade_packages)

Ansible role to upgrade all packages, process package manager cleanup, and reboot host if needed.

Requirements
------------

None.

Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

| Variable                          | Description           | Default |
|-----------------------------------|:----------------------|:--------|
| upgrade_packages_all              | Upgrade all packages  | true    |
| upgrade_packages_reboot_if_needed | Reboot host if needed | true    |

Dependencies
------------

None.

Example Playbook
----------------
```yaml
---
- hosts: servers
  roles:
    - { role: dtoch56.upgrade_packages }
```

License
-------

MIT / BSD

Author Information
------------------

This role was created in 2021 by dtoch.56.

Development
------------------
```bash
pip install pipenv
pipenv install
ansible-playbook main.yml --ask-become-pass
```
