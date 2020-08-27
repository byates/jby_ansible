Verilator
=========

Installs [Verilator](https://www.veripool.org/wiki/verilator) from source.

Requirements
------------

* prior devel install

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

Version to install: [List](https://github.com/verilator/verilator/tags)

    verilator_git_tag: "4.038"

Set to true to force install even if it already exists at the same version

    verilator_force_update: False

Dependencies
------------

none

Example Playbook
----------------
```
- name: Install Verilator
  hosts: hdl
  become: yes
  roles:
  - role: ansible-verilator
    verilator_git_tag: "4.038"
    verilator_force_update: true
```
License
-------

`MIT`

Author Information
------------------

brent.yates@gmail.com

