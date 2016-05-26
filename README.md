mjuenema.lxc
============

Ansible role for installing LXC either from system packages or its Git repository.

Requirements
------------

All packages that are required will be installed by the role.

Role Variables
--------------

The ```lxc_install_from_git``` variable determines whether LXC will be installed from
its Git repository or whether the package provided by the Linux distribution will
be used. The default is to use the packages provided by the Linux distribution. 

There are a number of general and distribution specific variables that are used. Check 
the ```defaults/main.yml``` and ```vars/*.yml``` files for details. 

Dependencies
------------

There are no dependencies on other Ansible roles.

Example Playbook
----------------

Install LXC through the packages provided by the Linux distribution.

    - hosts: servers
      roles:
         - { role: mjuenema.lxc }

License
-------

BSD

Supported distributions
-----------------------

This role is tested on the following Linux distributions.

* Fedora 23+
* CentOS 7+
* (more to come)

Status
------

Alpha

References
----------

The following references were used while developing this Ansible role.

* https://linuxcontainers.org/
* https://fedoraproject.org/wiki/LXC
* http://www.tecmint.com/install-create-run-lxc-linux-containers-on-centos/

Author Information
------------------

Markus Juenemann <markus@juenemann.net>
