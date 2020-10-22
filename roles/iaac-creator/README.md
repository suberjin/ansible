Role Name
=========

The role creates /etc/iaac file with 0500 permissions

Requirements
------------

This role could be run on Linux based hosts only

Role Variables
--------------

This role doesn't have any specific variables

Dependencies
------------

This role doesn't have any dependencies

Example Playbook
----------------

```
 - name: Create /etc/iaac - role
   hosts: iaas
   roles:
     - { role: 'iaac-creator', tags: 'iaac-creator' }
```

License
-------

BSD

Author Information
------------------

Akimov Vasiliy
