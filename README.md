# Ansible home task
=========

This is a home task. The mail.yml file invokes the roles. The first one creates an empty file /etc/iaac 
for two first servers in group `iaas`. The second one reads content of /etc/issue. In the end, playbook 
prints content of `/etc/issue` along with server hostname. 

Connection to ansible host is supposed to be via pasword. The ssh password is encrypted via Vault. 
The Vault password is `z8rWFJKACY3af3XwPmHp`

Requirements
------------

This role could be run on Linux based hosts only.


Example of Playbook running
----------------

```
ansible-playbook main.yml --ask-vault-pass 
```

License
-------

BSD

TODO
------------------

It is necessary to find out why the construction below gathers facts from localhost

```
---
- name: Read /etc/issue into variable
  set_fact:
    issue: "{{ lookup('file', '/etc/issue') }}"
```

Author Information
------------------

Akimov Vasiliy
