Role Name : Basic_installation
=========

Information about playbook:
-----------------------------
This playbook does the installation as follows
1. docker and docker compose (docker.yml)
2. dot Net (dot_net.yml)
3. Maven (maven.yml)
4. Tomact and java 11 (tomcat_and_java.yml)
5. Nodejs (nodejs.yml)
6. Nginx (nginx.yml)
7. Gunicorn (gunicorn.yml)

All these tasks are getting called in main.yml file

Role Variables
--------------
Variable File Name: Basic_installation/vars/main.yml
<!--
---
# vars file for jaydeep_product
maven_major: 3
maven_version: 3.6.3
maven_home_parent_directory: /opt
maven_env_file: "/etc/profile.d/maven.sh"


gunicorn_user_name: gunicorn
gunicorn_group_name: gunicorn

-->

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
<!--
- hosts: web
  roles:
    - Basic_installation
-->

Playbook run command:
----------------------
ansible-playbook product.yml -vvv



License
-------

BSD

Author Information
------------------
Rutuja Saste
