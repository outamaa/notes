# Ansible

## Pinging all hosts

``` shell
$ ansible all -m ping
```

## Minimal config

Use the `inventory` file from the current directory.

``` ini
[defaults]
inventory = ./inventory
```

## Bootstrapping the server

`bootstrap.yml`

``` yaml
---

- hosts: all
  gather_facts: False

  tasks:
  - name: install python 2
    raw: test -e /usr/bin/python || (apt -y update && apt install -y python)

...
```

``` shell
$ ansible-playbook bootstrap.yml
```
