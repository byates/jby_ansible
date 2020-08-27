Role Name
=========

Adds line to .bashrc to source jby-profile (in jbyconfig repo)

Requirements
------------

GIT repo jbyconfig is needed. It is installed into <home>if not already present.

Role Variables
--------------

none

Dependencies
------------

none

Example Playbook
----------------

- name: Install jby-profile link in bashrc
  hosts: all
  become: true
  roles:
  - role: jby-profile

License
-------

MIT

Author Information
------------------

brent.yates@gmail.com

