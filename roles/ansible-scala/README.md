Scala
=====

Ansible role that installs [Scala (SBT)](https://www.scala-lang.org/) to Ubuntu or Debian.

Requirements
------------

none

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

`sbt_version`

Which version of SBT to install (see [list)](https://www.scala-sbt.org/download.html)).

    sbt_version: "1.3.13"

`force_update`

Set to True to force the installation even if a previous verison exists.

    force_update: False

Dependencies
------------

none

Example Playbook
----------------

```
- name: Install Scala SBT
  hosts: devel
  roles:
  - role: ansible-scala
    vars:
      sbt_version: 1.3.13
      force_update: true
```

License
-------

The MIT License (MIT)

Copyright (c) 2020 Brent Yates

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Author Information
------------------

You can find me on [GitHub](https://github.com/byates/).
