Role Name
=========

Sets to the hostname to the specified value.

Requirements
------------

none

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

Name of the user:

    new_hostname: "{{ inventory_hostname }}"

Dependencies
------------

none

Example Playbook
----------------

- name: Set hostname
  hosts: all
  become: true
  roles:
  - role: set-hostname

License
-------

MIT

Author Information
------------------

brent.yates@gmail.com

