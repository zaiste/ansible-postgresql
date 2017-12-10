ansible-postgresql
=========

Ansible role that installs PostgreSQL for Ubuntu from the official APT. By default it supports Ubuntu 17.10

Requirements
------------

None.

Role Variables
--------------

- `dist` default to `zesty` (it compatible with `artful`)
- `databases` is a list; it defaults to `app` database owned by `app` user with `app` password (check the example playbook below)

Dependencies
------------

None.

Example Playbook
----------------

```yml
- hosts: servers
  roles:
  - role: zaiste.postgresql 
    databases:
    - name: app
      owner: app
      password: secr3t
      extensions:
      - hstore
    - name: data 
      owner: app
      extensions:
      - hstore 
      - isn 
```
           

License
-------

MIT / BSD

Author Information
------------------

[Zaiste](http://zaiste.net) 2017
