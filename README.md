Role Name
=========

Reference role for Molecule test


Requirements
------------

* Docker on the host. The role uses the docker driver
* Install molecule in a Python virtual environment
* pip install molecule[docker,lint,docker]
* molecule converge

Role Variables
--------------


Dependencies
------------

Example Playbook
----------------

    - hosts: servers
      tasks:
        - name: "Include acme.my_new_role"
          include_role:
          name: "acme.my_new_role"

License
-------

BSD

Author Information
------------------
Sudheer Satyanarayana
https://github.com/bngsudheer

https://www.techchorus.net - Blog
https://www.gavika.com - DevOps Consulting

