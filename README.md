# ansible-role-cmd

[![Build Status](https://travis-ci.org/EGI-Foundation/ansible-role-cmd.svg?branch=master)](https://travis-ci.org/EGI-Foundation/ansible-role-cmd)

Role for configuring CMD and OpenStack repositories


## Requirements

None

## Role Variables

* `cmd_distribution`: `cmd-os` for OpenStack, `cmd-one` for OpenNebula
* `cmd_openstack_release`: Release of OpenStack to use, default: `pike`
* `ca_verification: false` -  Enables the IGTF repository for trusted CAs (defaults to `false`)
* `ca_version: 1` : CA version (defaults to '1', only if `ca_verification: true`)
* `ca_branch: production` : CA branch (defaults to 'production', only if `ca_verification: true`)
* `ca_verification: true`: - CA servers (defaults to 'repository.egi.eu', only if
    `ca_verification: true`)
  * _e.g._ `ca_server: repository.egi.eu`
* `crl_deploy: false` : Installs 'fetch-crl' package if enabled (defaults to `false`)
  * _e.g._ : `crl_deploy: false`


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
