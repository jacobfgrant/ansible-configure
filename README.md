# ansible-configure

![Ansible Lint](https://github.com/jacobfgrant/ansible-configure/workflows/Ansible%20Lint/badge.svg?branch=master)

Ansible playbook to set up and configure a *nix machine.


# Properties

## Linux (Ubuntu)

Updates packages, configures UFW to allow SSH, creates a user, installs my [dotfiles repo](https://github.com/jacobfgrant/dotfiles), and installs a number of programs, including:

* Ansible
* Docker
* LaTeX
* Packer
* Python 3
* Serverless
* Terraform
* Vagrant
* Vim
* Zsh

If the machine includes a GUI, this playbook also installs:

* Discord
* Google Chrome
* Slack
* Visual Studio Code


## macOS

TODO


# Usage

This playbook is customized for me. I suggest you fork it and change it to fit your needs. You *probably* don't want my SSH public keys on your system.

To configure a machine using `ansible-pull`, you can run `sudo ansible-pull https://github.com/jacobfgrant/ansible-configure.git --connection=local --inventory 127.0.0.1, main.yml` on a system with Ansible installed.

Alternatively, you can run this playbook as you normally would using Ansible against any number of hosts.
