Role Name
=========

Installs tmux from source.

Requirements
------------

none

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

Version to install. See https://github.com/tmux/tmux.git

    tmux_git_tag: "3.0a"

When true, an AppImage will be downloaded and used. Otherwise tmux will be built from source.

    tmux_use_appimage: true

Set to true to force install even if it already exists at the same version

    tmux_force_update: False

Dependencies
------------

none

Example Playbook
----------------

- name: Install TMUX using AppImage
  hosts: devel
  become: yes
  roles:
  - role: ansible-tmux
    tmux_git_tag: "3.0a"
    tmux_use_appimage: true

- name: Install TMUX form source
  hosts: devel
  become: yes
  roles:
  - role: ansible-tmux
    tmux_git_tag: "3.0a"
    tmux_use_appimage: false
    tmux_force_update: False

License
-------

MIT

Author Information
------------------

brent.yates@gmail.com

