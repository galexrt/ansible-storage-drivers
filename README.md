ansible-storage-drivers
=======================

Ansible role for installation of storage drivers, like Ceph.

Requirements
------------

No special requirements.

Role Variables
--------------

```
# packages for debian and ubuntu
storage_drivers_ceph_packages_deb:
  - ceph-fs-common
  - ceph-common
# packages for not debian and ubuntu
storage_drivers_ceph_packages_rhel:
  - ceph

# if ceph "drivers" should be installed
storage_drivers_install_ceph: true
```

Dependencies
------------

No dependencies.

Example Playbook
----------------

An example playbook on how to use this role:

```
- hosts: servers
  roles:
     - { role: galexrt.storage-drivers, storage_drivers_install_ceph: true }
```

License
-------

MIT

Author Information
------------------

If you have problems with the role, feel free to create an issue on Github or contact me by mail.
