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
      tags: atom
```

License
-------

MIT

Author Information
------------------

- [Mihai Criveti](https://www.linkedin.com/in/crivetimihai/)

TODO
----

- Add Ubuntu and Debian support
