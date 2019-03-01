ansible-role-mat2-web
=====================

[![Build Status](https://travis-ci.org/systemli/ansible-role-mat2-web.svg?branch=master)](https://travis-ci.org/systemli/ansible-role-mat2-web)

Deploy [mat2-web](https://0xacab.org/jvoisin/mat2-web) as uWSGI service wih Ansible.

Features:

* Run mat2-web as a uWSGI service as dedicated system user
* Install bubblewrap to enable mat2 sandboxing
* Create a dm-crypt volume with random key for the uploads folder
* Install garbage collector cronjob, removes leftover files after five minutes

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
