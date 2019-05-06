# Apache Nifi Playbook

Playbook created to install and configure a single node of Apache Nifi, for development.

## Requirements

- Vagrant
- Ansible

## Install

```shell
$ vagrant up
```

With this the playbook:

- Install Java and define variable environment
- Download the Apache Nifi package
- Extract and move to `/usr/local`
- Define symbolic directory: `/opt/nifi`
- Define variable environment of Nifi to user `vagrant`
- Install the nifi service
- Start the service

To access the Nifi: `http://192.168.33.10:8080/nifi`
