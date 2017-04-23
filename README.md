# Ansible Role: ntp

An ansible role to install and configure ntp.

## Requirements

> This role has been tested on `Ubuntu 16.04` and `Ubuntu 16.10` only.

## Variables

- `ntp_timezone`: server timezone
  - Default: `Africa/Accra`
- `ntp_servers`: list of ntp servers for quorum
  - Default:
    ```yaml
    - 0.pool.ntp.org
    - 1.pool.ntp.org
    ```

## Usage Example

```yaml
- hosts: all
  vars:
    ntp_timezone: Africa/Accra
    ntp_servers:
      - 0.pool.ntp.org
      - 1.pool.ntp.org
  roles:
    - thedumbtechguy.ntp
```


## License

MIT / BSD

## Author Information

This role was created by [TheDumbTechGuy](https://github.com/thedumbtechguy) ( [twitter](https://twitter.com/frostymarvelous) | [blog](https://thedumbtechguy.blogspot.com) | [galaxy](https://galaxy.ansible.com/thedumbtechguy/) )

## Credits