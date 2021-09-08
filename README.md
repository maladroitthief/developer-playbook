---
title: Ubuntu developer playbook
description: An ansible playbook for setting up a developer machine
author: Ian Weller
date: 09.08.2021
---

# Ubuntu developer playbook

> Applies to me

## Before I begin

- [python3](https://www.python.org/downloads/)
- [ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html#installing-and-upgrading-ansible-with-pip)

## Run the playbook

First install the collections and roles roles required to run this playbook

```bash
ansible-galaxy install -r requirements.yaml
```

Run the playbook from the project root

```bash
ansible-playbook main.yaml --inventory inventory.yaml --ask-become-pass
```
