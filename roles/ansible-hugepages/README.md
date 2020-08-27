Role Name
=========

Set Linux (grub) command line settings to enable hugepages.
NOTE: This role changes the grub linux command line.

Requirements
------------

none

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

These variables set the _desired_ values for the number of huge pages.
Only one will be used with 1G having the highest preference (if supported by HW).
NOTE: If there is not enough memory for the desired value, a smaller value that fits
      will be used.

    desired_2m_pages: "4096"
    desired_1g_pages: "4"

Dependencies
------------

none

Example Playbook
----------------

- name: Install hugepage support for DPDK
  hosts: devel
  roles:
    - role: ansible-hugepages
      become: yes
      vars:
        desired_1g_pages: 4
        desired_2m_pages: 2048

License
-------

MIT

Author Information
------------------

brent.yates@gmail.com

