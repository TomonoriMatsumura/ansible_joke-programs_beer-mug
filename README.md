# Install beer-mug on CentOS7 with Ansible

## Introduction

This program installs [beer-mug](https://github.com/misoton665/beer-mug) on CentOS7.

## How To install

1. Install ansible

```
sudo yum -y install epel-release
sudo yum -y install ansible
```

2. Execute playbook as root

```
git clone https://github.com/TomonoriMatsumura/ansible_joke-programs_beer-mug.git
cd ansible_joke-programs_beer-mug
ansible-playbook -i localhost install.yml
```

## CircleCI Test Coverage

Test is executed on CircleCI with Docker container Centos7 latest Ansible installed: see Dockerfile [tomonorimatsumura/centos7-ansible](https://hub.docker.com/r/tomonorimatsumura/centos7-ansible/)

[![CircleCI](https://circleci.com/gh/TomonoriMatsumura/ansible_joke-programs_beer-mug.svg?style=svg)](https://circleci.com/gh/TomonoriMatsumura/ansible_joke-programs_beer-mug)
