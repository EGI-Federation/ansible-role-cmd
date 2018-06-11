# ansible-role-cmd

Role for configuring CMD and OpenStack repositories


## Requirements

None

## Role Variables

* `cmd_os_enable_rdo`: Whether to enable or not the setup of the RDO repositories, default: `true`
* `cmd_os_release`: Release of OpenStack to use, default: `pike`


## Dependencies

None

## Example Playbook

```yaml
    - hosts: servers
      roles:
         - { role: EGI-Foundation.cmd, cmd_os_release: queens }
```

## License

Apache-2.0

## Author Information

<!--
Add the relevant contributors
-->
