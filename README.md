at
=========

[![Build Status](https://travis-ci.org/robertdebock/ansible-role-at.svg?branch=master)](https://travis-ci.org/robertdebock/ansible-role-at)

Installs and enables at for your system.

[Unit tests](https://travis-ci.org/robertdebock/ansible-role-bootstrap) are done on every commit and periodically.

If you find issues, please register them in [GitHub](https://github.com/robertdebock/ansible-role-bootstrap/issues)

To test this role locally please use [Molecule](https://github.com/metacloud/molecule):
```
pip install molecule
molecule test
```
There are many scenarios available, please have a look in the `molecule/` directory.

Context
-------
This role is a part of many compatible roles. Have a look at [the documentation of these roles](https://robertdebock.nl/) for further information.

Here is an overview of related roles:
![dependencies](https://raw.githubusercontent.com/robertdebock/drawings/artifacts/at.png "Dependency")

Requirements
------------

Access to a repository containing packages, likely on the internet.

Role Variables
--------------

None known.

Dependencies
------------

This role can be used to prepare your system:

- [robertdebock.bootstrap](https://travis-ci.org/robertdebock/ansible-role-bootstrap)

Download the dependencies by issuing this command:
```
ansible-galaxy install --role-file requirements.yml
```

Compatibility
-------------

This role has been tested against the following distributions and Ansible version:

|distribution|ansible 2.4|ansible 2.5|ansible 2.6|ansible 2.7|ansible devel|
|------------|-----------|-----------|-----------|-----------|-------------|
|alpine-edge|yes|yes|yes|yes|yes|
|alpine-latest|yes|yes|yes|yes|yes|
|archlinux|yes|yes|yes|yes|yes|
|centos-6|yes|yes|yes|yes|yes|
|centos-latest|yes|yes|yes|yes|yes|
|debian-latest|yes|yes|yes|yes|yes|
|debian-stable|yes|yes|yes|yes|yes|
|fedora-latest|yes|yes|yes|yes|yes|
|fedora-rawhide|yes|yes|yes|yes|yes|
|opensuse-leap|yes|yes|yes|yes|yes|
|opensuse-tumbleweed|yes|yes|yes|yes|yes|
|ubuntu-artful|yes|yes|yes|yes|yes|
|ubuntu-latest|yes|yes|yes|yes|yes|

Example Playbook
----------------

The simplest way possible:
```
- hosts: servers

  roles:
    - robertdebock.bootstrap
    - robertdebock.at
```

Install this role using `galaxy install robertdebock.at`.

License
-------

Apache License, Version 2.0

Author Information
------------------

[Robert de Bock](https://robertdebock.nl/) <robert@meinit.nl>
