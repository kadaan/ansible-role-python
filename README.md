# Ansible Role: Python

[![Build Status](https://travis-ci.com/kadaan/ansible-role-python.svg?branch=master)](https://travis-ci.com/kadaan/ansible-role-python)

Installs python and global python packages.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    python_versions: []

Python versions you would like to make sure are installed by pyenv.

    python_pip_global_packages: []

Global PIP packages you would like to make sure are installed.

## Dependencies

  - [kadaan.homebrew](https://galaxy.ansible.com/kadaan/homebrew/)

## Example Playbook

    - hosts: localhost
      roles:
        - { role: kadaan.python, python_execute: true }

## License

Apache 2.0
