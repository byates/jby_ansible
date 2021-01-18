Role Name

=========

Installs vim configuration.

Requirements
------------

none

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

Name of the user to install the config files.

    target_username: "{{ ansible_user }}"

Dependencies
------------

none

Example Playbook
----------------

- name: Install vim config
  hosts: all
  roles:
  - role: jby-vim-config
    target_username: "{{ ansible_user }}"

License
-------

MIT

Author Information
------------------

brent.yates@gmail.com

