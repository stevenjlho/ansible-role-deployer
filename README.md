[![Build Status](https://travis-ci.org/stevenjlho/ansible-role-deployer.svg?branch=master)](https://travis-ci.org/stevenjlho/ansible-role-deployer)

Ansible role Deployer
=========

Ansible role for php [Deployer](http://deployer.org)

## Requirements

* PHP 5.5.0 and up.



Role Variables
--------------

    deployer_version: "3.3.0"
Set version of Deployer.



    deployer_path: "/usr/local/bin/dep"
The globally-accessible path of Deployer.



```
deployer_keep_upgrade: false
```

Set this to `true` to update Deployer to the latest release every time the playbook is run. Default is false.



```
deployer_force_upgrade: false
```

If Deploy already install an old version, set this to `true` to force upgrade Deployer according `deployer_version`. Default is false.


Dependencies
------------

none


Example Playbook
----------------

    - hosts: localhost
      remote_user: root
      roles:
        - stevenjlho.deployer


License
-------

MIT


Author Information
------------------

This role was created in 2016 by [Steven Ho](http://stevenjlho.github.io/)
