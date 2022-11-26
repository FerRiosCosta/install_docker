install_docker
=========

A role for quickly installing docker-ce on CentOS 9.

Requirements
------------

Only tested against CentOS 9.

Role Variables
--------------

docker_packages:
  \- "docker-ce"
  \- "docker-ce-cli"
  \- "docker-compose-plugin"
  \- "containerd.io"

docker_yum_repo_url: "https://download.docker.com/linux/centos/docker-ce.repo"

Dependencies
------------

None

Example Playbook
----------------

---
- name: Deploy app
  hosts: all
  roles:
    - install_docker
    - deploy_app


License
-------

BSD

Author Information
------------------

Author: Fernando Rios.
email: fer.rios.costa@gmail.com 
