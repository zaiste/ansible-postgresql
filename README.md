ansible-postgresql
=========

Ansible role that installs PostgreSQL for Ubuntu Xenial from the official APT.

Requirements
------------

None.

Role Variables
--------------

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

[Zaiste](http://zaiste.net) 2014 - 2016
