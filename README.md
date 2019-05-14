[![Build Status](https://travis-ci.com/zviederi/xymon-client.svg?branch=master)](https://travis-ci.com/zviederi/xymon-client)

Xymon Client
=========

Compile and install a xymon client on host machine from source

Requirements
------------

`Ansible >= 2.4`

Role Variables
--------------

```yaml
xymon_client_directory: "/usr/local"
```
Directory to install xymon client

```yaml
xymon_client_user_group: xymon
```
User group(default: xymon)

```yaml
xymon_server_address: 127.0.0.1
```
Xymon server IP address

Example Playbook
----------------

```yaml
- hosts: servers
- vars:
    xymon_server_address: 127.0.0.1
    xymon_client_user_group: xymon
  roles:  
    - xymon-client   # install xymon client
```

Author Information
------------------

* [Ēriks Zviedrāns](mailto:eriks.zviedrans@gmail.com)
