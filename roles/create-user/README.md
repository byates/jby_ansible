Role Name
=========

Creates a user with specific group membership and ssh keyfile.

Requirements
------------

none

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

Name of the user:

    target_username: "user"

Which groups the user will be a member of.

    user_groups:
      - sudo
      - wheel
      - hugepage

The user_pass variable is used to set the users's password. Must be encrypted. Easiest way to get
an encrypted value is to read the /etc/shadow file (must be su)

    user_pass: <encrypted_string>

Location on the host server of the public keyfile to add to the users authorized_key file.
REQUIRED to be set.

    user_keyfile:

Dependencies
------------

none

Example Playbook
----------------

- name: Create user
  hosts: all
  become: true
  roles:
  - role: create-user
    target_username: "user"
    user_keyfile: "~/.ssh/id_rsa.pub"

License
-------

MIT

Author Information
------------------

brent.yates@gmail.com

