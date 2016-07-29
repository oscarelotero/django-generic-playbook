===================================
Django Generic Playbook for Ansible
===================================

This is a basic setup for deployment to a server on EC2. Currently it
installs system dependencies, creates a virtualenv and installs python
dependencies. 

It has been tested on projects using Django Cookiecutter structure.

************
Requirements
************

* Python >= 2.7
* Ansible 2.1

***********
Get started
***********

The repository comes with a hosts.example file for reference. Copy, edit and reference this file when running the playbook.


Configure the hosts file
========================
::

    [project_name]
    server_host

    [project_name:vars]
    ansible_ssh_user=ubuntu
    ansible_ssh_private_key_file=/path/to/key.pem
    repo_url=ssh://git@github.com/repository_name.git
    app_name=app_name
    server_name='server_host'


Run in the console
==================

::

    ansible-playbook playbook.yml –extra-vars “repo\_tag commit\_hash”
