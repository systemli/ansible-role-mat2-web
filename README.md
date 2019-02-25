ansible-role-mat2-web
=====================

[![Build Status](https://travis-ci.org/systemli/ansible-role-mat2-web.svg?branch=master)](https://travis-ci.org/systemli/ansible-role-mat2-web)

Deploy [mat2-web](https://0xacab.org/jvoisin/mat2-web) as uWSGI service wih Ansible.

Contains tests for Travis CI, Molecule and Vagrant.

Requirements
------------

Debian 9. Other versions of Debian/Ubuntu might be supported as well, but aren't tested.


Tests
-----

Run local tests with
```
molecule test
```
Requires Molecule, Vagrant and `python-vagrant` to be installed.

License
-------

GPLv3

Author Information
------------------

https://www.systemli.org
