Ansible AWX Role
=========

Ansible role to deploy Ansible AWX on a CentOS 7 host.

Requirements
------------

Host that AWX will be deployed on is running CentOS 7.

Role Variables
------------

Role variables are listed below with default values (see `defaults/main.yml`):

    awx_repo: https://github.com/ansible/awx.git
    awx_repo_dir: "~/awx"
    awx_version: 2.0.1

Dependencies
------------

N/A

Example Playbook
----------------

    - hosts: awx
      roles:
         - ansible-awx-role

License
-------

MIT/BSD

Author Information
------------------

This role was created by [Michael Tipton](https://ibeta.org).
