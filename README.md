Ansible AWX Role
=========

Ansible role to deploy Ansible AWX on a CentOS 7 host with options of container based, local, or remote postgresql server.

Requirements
------------

Host that AWX will be deployed on is running CentOS 7.

Role Variables
------------

Role variables are listed below with default values (see `defaults/main.yml`):

    awx_repo: https://github.com/ansible/awx.git
    awx_repo_dir: "~/awx"
    awx_version: 2.0.1

If awx_db_type is undefined the default is:

    awx_db_type: container

Other options for awx_db_type:
    
    awx_db_type: local
    awx_db_type: remote
    
If awx_db_type is set to `remote` an additional variable is required:

    pg_hostname: postgresdb.host.local


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
