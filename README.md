Role Name
=========

Ansible role to install and configure Salt.

Requirements
------------
- None

Role Variables
--------------
Set the daemons to install on the master node. 
```yaml
# group_vars/masters.yml
salt_daemons:
  - "salt-master"
  - "salt-minion"
```
  
Minions daemons are already defined in the defaults

Dependencies
------------
- None

Example Playbook
----------------
```yaml
- hosts: all
  become: True

  roles:
    - role: ansible-saltstack
```

License
-------
GPLv3

Author Information
------------------
- BobTheButcher

