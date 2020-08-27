Role Name

=========

Installs nvim JBY configuration.

Requirements
------------

none

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

Name of the user to install the config files.

    target_username: "user"

Dependencies
------------

none

Example Playbook
----------------

- name: Install nvim JBY config
  hosts: all
  become: true
  roles:
  - role: jby-nvim-config
    target_username: "user"

License
-------

MIT

Author Information
------------------

brent.yates@gmail.com

