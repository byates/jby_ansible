protobuf-install
================

Install Google Protocol Buffers compiler.

Requirements
------------

None.

Role Variables
--------------

protoc_checksum: Checksum for Google protocol buffers compiler binary.
protobuf_version: Version of Google protocol buffers to install.

Dependencies
------------

None.

Example Playbook
----------------

None.

    - hosts: servers
      roles:
         - role: lfit.protobuf-install
           protobuf_version: 4.0.0-rc2
           protobuf_name: 4.0.0-rc-2
           protoc_checksum: sha256:568ae47c4fd83281c4c76d6c3c96d9ba45704f220bb6ce4197b9f86aba05848c

License
-------

MIT

Author Information
------------------

Linux Foundation Release Engineering
