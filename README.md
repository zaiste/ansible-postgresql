ansible-postgresql
=========

Ansible role that installs PostgreSQL for Ubuntu from the official APT. By default it supports Ubuntu 17.10

Requirements
------------

None.

Role Variables
--------------

- `dist` default to `artful`
- `postgresql_user` defaults to `app`
- `postgresql_password` defaults to `app`
- `postgresql_database` defaults to `app`

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: zaiste.postgresql }

License
-------

MIT / BSD

Author Information
------------------

[Zaiste](http://zaiste.net) 2017
