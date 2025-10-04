rpi_avahi
=========
[![Ansible Lint](https://github.com/oxivanisher/role-rpi_avahi/actions/workflows/ansible-lint.yml/badge.svg)](https://github.com/oxivanisher/role-rpi_avahi/actions/workflows/ansible-lint.yml)

Enable or disable the avahi daemon by masking its systemd unit and triggering socket.

As always: Use at your own risk!

Role Variables
--------------

| Name              | Comment                              | Default value |
| ----------------- | ------------------------------------ | ------------- |
| rpi_avahi_disable | Should the avahi daemon be disabled? | `true`        |

Example Playbook
----------------

```yaml
- name: Enable or disable avahi daemon on Raspberry Pi
  hosts: rpis
  collections:
    - oxivanisher.raspberry_pi
  roles:
    - role: oxivanisher.raspberry_pi.rpi_avahi
```

License
-------

BSD

Author Information
------------------

This role is part of the [oxivanisher.raspberry_pi](https://galaxy.ansible.com/ui/repo/published/oxivanisher/raspberry_pi/) collection, and the source for that is located on [github](https://github.com/oxivanisher/collection-raspberry_pi).
