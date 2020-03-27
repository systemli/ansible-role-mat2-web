ansible-role-mat2-web
=====================

[![Build Status](https://travis-ci.org/systemli/ansible-role-mat2-web.svg?branch=master)](https://travis-ci.org/systemli/ansible-role-mat2-web)
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

Debian 10. Other versions of Debian/Ubuntu might be supported as well, but aren't tested.


Tests
-----

For developing and testing the role we use Travis CI, Molecule and Vagrant. On the local environment you can easily test the role with

```
pip install molecule-vagrant ansible-lint yamllint
molecule test
```

This requires [Vagrant](https://www.vagrantup.com/downloads.html) to be installed.

License
-------

GPLv3

Author Information
------------------

https://www.systemli.org
