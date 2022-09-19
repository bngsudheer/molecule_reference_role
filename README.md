Role Name
=========

Reference role for Molecule test


Requirements
------------

* Docker on the host. The role uses the docker driver

Installation And Usage
-----------------------
```shell
python3 -m venv ansible-env # you may have to uninstall other Ansible and molecule installations on your host
source ansible-env/bin/activate
pip install molecule[docker,lint,docker] ansible-lint
# cd molecule_reference_role/ # this repository root
molecule converge
```
* Install molecule in a Python virtual environment
* 
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

