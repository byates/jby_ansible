Role Name
=========

Installs vim from source.

Requirements
------------

none

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

Version to install. See https://github.com/vim/vim.git

    vim_git_tag: "v8.2.2374"
     or
    vim_git_tag: "HEAD"

Version to check. If <major><minor> doesn't match, VIM will be build from source.

    vim_version: "8.2"

Set to true to force install even if it already exists at the same version

    vim_force_update: False

Dependencies
------------

none

Example Playbook
----------------

- name: Install vim form source
  hosts: devel
  become: yes
  roles:
  - role: ansible-vim
    vim_git_tag: "HEAD"
    vim_version: "8.2"
    vim_force_update: False

License
-------

MIT

Author Information
------------------

brent.yates@gmail.com

