# ansible_role_tripleo_undercloud

A role to configure and install the Undercloud as part of an OpenStack deployment using TripleO.

## Requirements

* Ansible >= 2.7

## Dependencies

None.

## Role Variables

* openstack_release = The OpenStack release to setup on the Undercloud. Default: rocky.
* openstack_repo = The OpenStack RPM repository to use: "centos" or "rdo". Default: rdo.
* tripleo_undercloud_install = If the "openstack undercloud install" command should be executed. Default: False.
* tripleo_undercloud_upload_images = If the Overcloud kernel, initramfs, and QCOW2 image should be automatically downloaded and uploaded to Glance. Default: False.
* tripleo_undercloud_config = Custom configurations for the Undercloud.

## Example Playbook

```
---
- hosts: undercloud
  roles:
    - ansible_role_tripleo_undercloud
```

## License

Apache v2.0
