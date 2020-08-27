Role Name
=========

Simple role to update all installed packages.

Requirements
------------

none

Role Variables
--------------

none

Dependencies
------------

none

Example Playbook
----------------

- name: Update all packages
  hosts: all
  become: true
  roles:
  - role: ansible-pkg-update

License
-------

MIT

Author Information
------------------

brent.yates@gmail.com

