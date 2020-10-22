Role Name
=========

The role reads /etc/issue file into variable

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
 - name: Show the issue content
   hosts: all
   roles:
     - { role: 'issue-reader', tags: 'issue-reader' }
```

License
-------

BSD

Author Information
------------------

Akimov Vasiliy
