# ansible-role-cmd

[![Build Status](https://travis-ci.org/EGI-Foundation/ansible-role-cmd.svg?branch=master)](https://travis-ci.org/EGI-Foundation/ansible-role-cmd)

Role for configuring CMD and OpenStack repositories


## Requirements

None

## Role Variables

* `cmd_distribution`: `cmd-os` for OpenStack, `cmd-one` for OpenNebula
* `cmd_openstack_release`: Release of OpenStack to use, default: `pike`


## Dependencies

None

## Example Playbook

```yaml
    - hosts: servers
      roles:
         - { role: EGI-Foundation.cmd, cmd_openstack_release: queens }
```

## License

Apache-2.0

## Author Information

<!--
Add the relevant contributors
-->
