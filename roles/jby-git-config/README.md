Role Name
=========

Installs jbyconfig repo and add include directive to <user>.gitconfig to
point

Requirements
------------

GIT repo jbyconfig is needed. It is installed into <home>if not already present.

Role Variables
--------------

Name of the user:

    new_hostname: "{{ inventory_hostname }}"

Dependencies
------------

none

Example Playbook
----------------

- name: Add include directive to .gitconfig to jbyconfig
  hosts: all
  become: true
  roles:
  - role: jby-git-config
    target_username: byates

License
-------

MIT

Author Information
------------------

brent.yates@gmail.com

