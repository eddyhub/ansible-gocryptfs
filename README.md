ansible-gocryptfs
=========

[![BSD License](http://img.shields.io/badge/license-BSD-blue.svg)](http://opensource.org/licenses/BSD-3-Clause)
[![Build Status](https://travis-ci.org/eddyhub/ansible-gocryptfs.svg?branch=master)](https://travis-ci.org/eddyhub/ansible-gocryptfs)

Ansible role for managing gocryptfs installation from https://nuetzlich.net/gocryptfs/

Installation
------------

ansible-galaxy install eddyhub.gocryptfs

Requirements
------------

None.

Role Variables
--------------

```yaml
---
# defaults file for ansible-gocryptfs

ansible_unit_test: false
gocryptfs_role_release: '0.0.1'

# gocryptfs version to install
gocryptfs_version: 'latest'

# gocryptfs platform
gocryptfs_platform: 'amd64'

# gocryptfs name with installed version
gocryptfs_name: 'gocryptfs'

# gocryptfs install directory
gocryptfs_install_directory: '/usr/local/bin'

# gocryptfs owner
gocryptfs_owner: 'root'

# gocryptfs group
gocryptfs_group: 'root'

# gocryptfs set suid access
gocryptfs_mode: '4755'
```

Dependencies
------------

None, for role to install.

Example Playbook
----------------

```yaml
- name: Installing Gocryptfs
  hosts: all
  sudo: yes
  roles:
    - role: eddyhub.gocryptfs
```

License
-------

Copyright (c) 2016, Eduard Angold
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

* Redistributions of source code must retain the above copyright notice, this
  list of conditions and the following disclaimer.

* Redistributions in binary form must reproduce the above copyright notice,
  this list of conditions and the following disclaimer in the documentation
  and/or other materials provided with the distribution.

* Neither the name of ansible-gocryptfs nor the names of its
  contributors may be used to endorse or promote products derived from
  this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

Author Information
------------------

eddyhub@users.noreply.github.com
