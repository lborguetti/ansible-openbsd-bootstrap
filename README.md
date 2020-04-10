ansible-openbsd-bootstrap
=========

Install Python on OpenBSD. Ansible is agentless by default, however, it requires Python on managed nodes

Requirements
------------

None.

Role Variables
--------------

**python_interpreter:** the path to python interpreter, used by check if python have already been installed.

**python_version:** the version of python that will be installed.

Default value:

```
python_interpreter: /usr/local/bin/python3
python_version: python-3.7.4
```

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      gather_facts: no
      roles:
         - { role: openbsd-bootstrap }

License
-------

ISC
