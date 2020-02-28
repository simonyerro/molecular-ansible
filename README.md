# Ansible and Molecule

Simple overview of Ansible and Molecule

## Description

### Ansible

Ansible is an open-source tool that allows you to manage, infrastructure by automating deployment in multiple environments.
In other words, you can easily execute scripts to remote servers via ssh.
It a simpler tool to learn and use compared to its contestant (Salt, Chef, Puppet)

### Molecule

[to complete]

### Ansible-lint

[to complete]

## Getting Started

### Dependencies

Ansible support Windows machine but the Master has to be on Linux/Unix machine

### Installing

#### Master

You'll need a few things to install like:
* python and pip (ansible is based on python and pip is the package manager associated)
* docker and vagrant

You'll find the packages to install in the script file

#### Remote

The remote servers where ansible will be deployed will only need to have python.

```bash
sudo apt install python
```

### Executing program

```bash
# To verify that the connection is established well with the hosts
ansible ec2 -i inventory -m ping
# To run the playbook 
ansible-playbook main.yml -i inventory --tags "mongo"
```

## Authors

Contributors names and contact info

ex. [@simonyerro](https://www.linkedin.com/in/simon-yerro/)

## Acknowledgments

Inspiration, code snippets, etc.
* [based on this tuto](https://www.objectif-libre.com/fr/blog/2019/01/15/ansible-molecule/)
