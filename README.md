# About

Just a tiny repository to help install Dokuwiki everywhere

# Usage

## Development

### Requirements

* [VirtualBox 4.3.18](http://download.virtualbox.org/virtualbox/4.3.18/)
* [Vagrant 1.7.2](http://www.vagrantup.com/download-archive/v1.7.2.html)
* [Ansible 1.8.2](http://releases.ansible.com/ansible/)
* [ansible-roles](http://github.com/ryankanno/ansible-roles/)

You may need to tweak your ansible.cfg.  See an [example ansible.cfg](https://github.com/ryankanno/ansible-dokuwiki/blob/master/ansible.cfg.example)
that I use.

### Getting started

`vagrant up`

The guest's port 80 is being forwarded to the host's port 50000.

    config.vm.network "forwarded_port", guest: 80, host: 50000, auto_correct: true

To play with the install from your machine,

`curl http://127.0.0.1:50000/`

# TODO

* Fix permissions to lib/plugins (should give web permission to write into the folder to install plugins)
* Add SSL
