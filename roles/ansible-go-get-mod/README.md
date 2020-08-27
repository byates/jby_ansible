Role Name
=========

Installs Golang MODULES (GO111MODULE="on")

Requirements
------------

Go must be installed.

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

This is the list of modules to install. Each should have a `name` and a `url`. The `force`
parameter is optional.

    mod_list: []

Set to True to force the installation even if a previous verison exists.

    force: False

Dependencies
------------

none

Example Playbook
----------------

- name: Install Go module lazygit
  hosts: devel
  become: "{{ target_user != active_user }}"
  become_user: "{{ target_user }}"
  roles:
  - role: ansible-go-get
    mod_list:
    - name: lazygit
      url: github.com/jesseduffield/lazygit
      force: True

License
-------

MIT

Author Information
------------------

brent.yates@gmail.com

