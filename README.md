[![Build Status](https://travis-ci.org/marvel-nccr/ansible-role-bigdft.svg?branch=master)](https://travis-ci.org/marvel-nccr/ansible-role-bigdft)
# Ansible Role: marvel-nccr.bigdft

An Ansible role that installs [BigDFT](https://bigdft.org) on Ubuntu.

## Installation

`ansible-galaxy install marvel-nccr.bigdft`

## Role Variables

See `defaults/main.yml`

## Example Playbook

```yaml
  - hosts: servers
    roles:
    - role: marvel-nccr.bigdft
```

## License

MIT - BigDFT code is licensed under GNU GPL v2

## Contact

Please direct inquiries regarding Quantum Mobile and associated ansible roles to the [AiiDA mailinglist](http://www.aiida.net/mailing-list/).
