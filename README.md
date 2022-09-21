Role Name
=========

Reference role for Molecule test

[Youtube Video Of Screen Recording](https://www.youtube.com/watch?v=_4QTRvZDiG8)

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
yamllint .
molecule lint
molecule converge
MOLECULE_PLAYBOOK=http-port.yml
molecule test
```

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

