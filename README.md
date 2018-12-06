# ansible_role_tripleo_undercloud

A role to configure and install the Undercloud as part of an OpenStack deployment using TripleO.

## Requirements

* Ansible >= 2.5

## Dependencies

None.

## Role Variables

* openstack_release = The OpenStack release to setup on the Undercloud. Default: rocky.
* openstack_repo = The OpenStack RPM repository to use: "centos" or "rdo". Default: rdo.
* tripleo_undercloud_install = If the "openstack undercloud install" command should be executed. Default: False.

## Example Playbook

```
---
- hosts: undercloud
  roles:
    - ansible_role_tripleo_undercloud
```

## License

Apache v2.0
