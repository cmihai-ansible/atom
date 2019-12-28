Role Name
=========

atom

[![Build Status](https://travis-ci.org/cmihai-ansible/atom.svg?branch=master)](https://travis-ci.org/cmihai-ansible/atom)

Ansible galaxy:
---------------

[https://galaxy.ansible.com/crivetimihai/atom](https://galaxy.ansible.com/crivetimihai/atom)

```bash
ansible-galaxy install crivetimihai.atom
```

Requirements
------------

- For RHEL, a Red Hat subscription or functional local repository.

Role Variables
--------------

```
atom_remove_packages: true
atom_enable_service: true
atom_enable_selinux: true
atom_firewall_configure: true
atom_firewall_rules:
  - service:
```

Dependencies
------------

- For Red Hat, subscription-manager.

Example Playbook
----------------

```yaml
---
- name: Install atom on localhost
  hosts:
    - localhost
  connection: local

  tasks:
    - name: atom is configured
      import_role:
        name: crivetimihai.atom
      vars:
        atom_remove_packages: true
        atom_enable_service: true
        atom_firewall_configure: true
        atom_firewall_rules:
          - service:
      tags: atom
```

License
-------

MIT

Author Information
------------------

- [Mihai Criveti](https://www.linkedin.com/in/crivetimihai/)
