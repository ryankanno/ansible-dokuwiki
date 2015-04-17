# About

Just a tiny repository to help install Dokuwiki everywhere

# Usage

## Development

### Requirements

* [VirtualBox 4.3.18](http://download.virtualbox.org/virtualbox/4.3.18/)
* [Vagrant 1.7.2](http://www.vagrantup.com/download-archive/v1.7.2.html)
* [Ansible 1.8.2](http://releases.ansible.com/ansible/)

### Getting started

`vagrant up`

The guest's port 80 is being forwarded to the host's port 50000.

    config.vm.network "forwarded_port", guest: 80, host: 50000, auto_correct: true

To play with the install from your machine,

`curl http://127.0.0.1:50000/`

# TODO

* Add SSL
