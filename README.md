Role Name
=========

A simple Ansible role that installs Vector on a Debian-based machine and configures it using a template file.

Requirements
------------

None

Role Variables
--------------

| Variable | Description |
| -------- | ----------- |
| vector_version | A vector version to be installed |
| vector_pkg_arch | A package architecture |
| vector_deb_pkg | Download path to the desired vector package |
| vector_config_path | Path to the vector config file |

Dependencies
------------

None

Example Playbook
----------------

```
- name: Install Vector
  hosts: vector
  become: true
  roles:
    - vector
```

License
-------

MIT
