Role Name:
=========

Setting up a preivate Docker repository using Ansible Playbook

Requirements:
------------

- Expects CentOS/RHEL 7.x based system
- Minimum Ansible Version : 1.2

This playbook installs Docker CE on RHEL/CentOS 7.x based systems and then creates a private repository. To use this, first edit the "inventory" file to contain the hostname of the system where docker is to be installed. Also the variables under group_vars/all.yml should be updated accordingly.

Running the Playbook:
----------------

To run the playbook, use this:

- Update inventory file for IP-ADDRESS, USER-NAME and SSH PRIVATE KEY FILE
- Update the variables under group_vars/all.yml

then run the below command to install Docker CE & setup private registry.

ansible-playbook docker-private-registry.yml -i inventory

License
-------

BSD

Author Information
------------------

Diptajeet Khan
