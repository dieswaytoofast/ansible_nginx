Role Name
=========

Collection of utils to install and run [nginx](https://www.nginx.com/) in docker
Note that the files in `sys` are wat you'll need to have in the playbooks that you'll be including ansible_nginx in
(Look at [elk-docker](https://github.com/dieswaytoofast/elk-docker/tree/master/ansible/sys) for an example

Requirements
------------

Requires Ansible 2.1 or higher.

Role Variables
--------------

Depends on the specific command being run.
Include
   * `paths.weave`  (path to `weave` command, probably `/usr/local/bin/weave`.
   * `weave_name` (parameter passed in, probably for get_container_ip_addr.yml`



Dependencies
------------

Probably docker :-)
Oh. and weave.

Example Playbook
----------------

    - hosts: foo
      roles:
         - role: dieswaytoofast.ansible_nginx

License
-------

BSD

Author Information
------------------

Mahesh Paolini-Subramanya (@dieswaytoofast)
