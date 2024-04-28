# rpi_cluster

This repository contains ansible scripts utilized to administer my personal

## Setup

Install Ansible

```zsh
pip install -U ansible ansible-lint
```

## Useful Commands

Ping all hosts

```zsh
ansible all -m ping
```

----


Update software on all machines

```zsh
ansible-playbook -i hosts.yaml ./playbooks/update_packages.yaml
```

----

Reboot all hosts

```zsh
ansible all -a "/sbin/reboot" --become
```