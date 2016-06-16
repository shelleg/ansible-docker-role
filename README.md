Role Name
=========

A brief description of the role goes here.

Requirements
------------
if using a secure private registry you will have to set the variable secure_registry to True and  provide ansible with the signed certificate (can be a self signed one) and put it in 
vars folder with the name vars/registrycrt.yml. you should provide it encrypted with vault. 
run ansible-vault encrypt vars/registrycrt.yml

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------
You can pass role parameters inside the playbook
  - hosts: docker_host
    roles:
      - { role: docker_host, secure_registry: True }

You can also use group/host vars for that as usual in the inventory file.

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
