Role Name
=========

Installs nvim via snaps

Requirements
------------

none

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

Which nodejs version to install.

    node_version: "13"

If true, install diff-so-fancy via npm

    install_dsf: true

Dependencies
------------

none

Example Playbook
----------------

- name: Install nvim via snaps
  hosts: all
  become: true
  roles:
  - role: ansible-nvim-snap
    node_version: "13"
    install_dsf: true

License
-------

MIT

Author Information
------------------

brent.yates@gmail.com

