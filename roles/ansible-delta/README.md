Role Name
=========

Installs the 'delta' utility for better git diffs.

Requirements
------------

none

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

Version to install. See https://github.com/sharkdp/bat/releases:

    delta_version: "0.12.1"

Where to put the binary:

    delta_dest: "/usr/bin"

Set to true to force install even if delta exists at the same version

    force_update: False

Dependencies
------------

none

Example Playbook
----------------

- name: Install Delta
  hosts: devel
  roles:
  - role: ansible-delta
    become: yes

License
-------

MIT

Author Information
------------------

brent.yates@gmail.com

