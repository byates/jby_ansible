svlint
=========

Installs [svlint](https://github.com/dalance/svlint) from binary archive.

Requirements
------------

* prior devel install

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

Version to install: [List](https://github.com/dalance/svlint/releases/latest)

    svlint_git_tag: "0.4.7"

Set to true to force install even if it already exists at the same version

    svlint_force_update: False

Dependencies
------------

none

Example Playbook
----------------
```
- name: Install svlint
  hosts: hdl
  become: yes
  roles:
  - role: ansible-svlint
    svlint_git_tag: "0.4.7"
    svlint_force_update: true
```
License
-------

`MIT`

Author Information
------------------

brent.yates@gmail.com

