Arcanist
=========

Ansible role to install [arcanist](https://github.com/phacility/arcanist) linux

Requirements
------------
- Ansible Core >= 2.16
- Tested Linux Distribution
  - Debian 12
  - Ubuntu 24.04
  - Fedora 40

> Note: Other distributions likely to work but not been tested

Role Variables
--------------

The following variables will change the behavior of this role (default values are shown below):

```yaml
# commit version of arcanist (HEAD, or SHA-1 commit hash)
# arcanist_commit_hash: e50d1bc4eabac9c37e3220e9f3fb8e37ae20b957
arcanist_commit_hash: HEAD

# arcanist install (clone from repository)
arcanist_install_dir: /opt/arcanist

# option (present,absent)
arcanist_state: present
```


Example Playbook
----------------
```yaml
- hosts: servers
  roles:
    - role: labasubagia.arcanist
```

License
-------

MIT

Author Information
------------------

[Laba Subagia](https://github.com/labasubagia)
