ansible-role-mat2-web
=====================

[![Build Status](https://github.com/systemli/ansible-role-mat2-web/workflows/Integration/badge.svg?branch=master)](https://github.com/systemli/ansible-role-mat2-web/actions?query=workflow%3AIntegration)
[![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-mat2__web-blue.svg)](https://galaxy.ansible.com/systemli/mat2_web/)

Deploy [mat2-web](https://0xacab.org/jvoisin/mat2-web) as uWSGI service wih Ansible.

Features:

* Run mat2-web as a uWSGI service as dedicated system user
* Install bubblewrap to enable mat2 sandboxing
* Create a dm-crypt volume with random key for the uploads folder
* Install garbage collector cronjob, removes leftover files after five minutes
* Install custom html templates

Contains tests for Travis CI, Molecule and Vagrant.

Requirements
------------

Debian 10 or Debian 11. Other versions of Debian/Ubuntu might be supported as well, but aren't tested.


Testing & Development
---------------------

Tests
-----

For developing and testing the role we use Github Actions, Molecule, and Vagrant. On the local environment you can easily test the role with

Run local tests with:

```
molecule test
```

Requires Molecule, [Vagrant](https://www.vagrantup.com/downloads.html)  and `python-vagrant, molecule-goss, molecule-vagrant` to be installed.For developing and testing the role we use Travis CI, Molecule and Vagrant. On the local environment you can easily test the role with

This will spin up a virtual machine with Debian Buster. Afterwards you can connect to the mat2
web interface via:

```
http://localhost:8080
```


License
-------

GPLv3

Author Information
------------------

https://www.systemli.org
