# Warning
This project is under development and is not yet tested in any other that a
vagrant box. Use at own risk!

# Install guide

This setup includes to following:
- Create a sudo, passwordless user, prevent root login
- Ip-tables, git
- Install ruby, rbenv, ruby-build

# Runned commands

## Install. but ask for ssh-password
basic setup: `ansible-playbook -i ansible_hosts setup.yml -k`

other setup: `ansible-playbook -i ansible_hosts tasks/ruby.yml tasks/your_application.yml`

## Ip-tables setup
http://deangerber.com/blog/2011/09/10/basic-iptables-firewall-configuration/

# Configuration files
Within the variables folder are *.example.yml files. Use these as templates to create
your own configuration.

ssh-copy-id root@host

