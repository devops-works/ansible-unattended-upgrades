# role-unattended-upgrades

Configures host to apply automatic security upgrades.

## Variables

- `unattended_blacklisted_packages`: list of packages to skip when
    applying unattended upgrades

`unattended_blacklisted_packages` defaults to the following packages
list:

- graylog-*
- openjdk-*
- java-*
- elasticsearch
- mongodb-*
- docker-*
- cassandra

## Platforms

This role only applies to ubuntu server (LTS >= 16.04).

## Using the role

```yaml
- hosts: all
  roles:
    - role-unattended-upgrades
```

## License

Internal use only. Requires licence & code review before going public.

## Author Information

@DevOps.Works
