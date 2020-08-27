Role Name
=========

Installs the 'bat' utility and extras.

Requirements
------------

none

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

Version to install. See https://github.com/sharkdp/bat/releases:

    bat_version: "0.12.1"

Where to put the binary:

    bat_dest: "/usr/bin"

Dependencies
------------

none

Example Playbook
----------------

- name: Install bat
  hosts: devel
  roles:
  - role: ansible-bat
    become: yes

License
-------

MIT

Author Information
------------------

brent.yates@gmail.com

