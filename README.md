ansible-role-pg-partman
=======================

![Molecule Test](https://github.com/kevincoakley/ansible-role-pg-partman/workflows/Molecule%20Test/badge.svg)

Installs the pg_partman partition management extension for PostgreSQL 10 - https://github.com/pgpartman/pg_partman . Tested with pg_partman 3.2.1 on CentOS 7.

Requirements
------------

None

Role Variables
--------------

See defaults/main.yml and the example inventory below

Dependencies
------------

None

Example Playbook
----------------

    - name: Install PG_PARTMAN for PostgreSQL 10
      hosts: partman
      become: yes
      become_method: sudo
    
      roles:
        - ansible-role-pg-partman
    
      tags:
        - partman

License
-------

BSD

Author Information
------------------

Kevin Coakley (https://github.com/kevincoakley)