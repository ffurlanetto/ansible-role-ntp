# ansible-role-connectivity-check

This role do a connectivity check and validate the the playbook can execute commands as root (become)

Requirements
------------

Python 3.5 or above (Ansible 2.5 requirement).

Dependencies
------------

See `meta/main.yml` for other roles dependencies

Example Playbook
----------------

```yaml
---
- hosts: all
  roles:
    - ansible-role-connectivity-check
```

Tests
-----

Test are made via Molecule and TestInfra. They will be automatically ran by the CI after every push. For a local run

- Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
- Install [Vagrant](https://www.vagrantup.com/downloads.html)
- Open a command prompt in the repository local folder and run `vagrant up`
- Wait for it to be done starting & configuring & provionning, then `vagrant ssh`
- Once connected in the VM, testing molecule is `cd /vagrant/ansible-role-YOUR_ROLE_NAME_HERE; molecule test`

Author Information
------------------

Florian Furlanetto - florian.furlanetto@visium360.com
