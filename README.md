# Message of The Day (MOTD) Role for Ansible

[![Build Status](https://travis-ci.org/petemcw/ansible-role-motd.svg?branch=master)](https://travis-ci.org/petemcw/ansible-role-motd)

This role manages the Message of The Day.

## Role Variables

The variables that can be passed to this role and a brief description about
them are as follows:

```yaml
# Custom MOTD text
motd_message: ""

# MOTD ASCII template 
motd_template: "empty"
```

## Examples

1. Configure the MOTD with the defaults:

    ```yaml
    ---
    # This playbook configures MOTD

    - name: Configure MOTD on all nodes
      hosts: all
      roles:
        - motd
      vars:
        motd_message: "Powerful you have become."
        motd_template: "yoda"
    ```

## License

MIT
