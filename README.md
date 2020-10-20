[![CI](https://github.com/marvel-nccr/ansible-role-bigdft/workflows/CI/badge.svg)](https://github.com/marvel-nccr/ansible-role-bigdft/actions)
[![Ansible Role](https://img.shields.io/ansible/role/37783.svg)](https://galaxy.ansible.com/marvel-nccr/bigdft)
[![Release](https://img.shields.io/github/tag/marvel-nccr/ansible-role-bigdft.svg)](https://github.com/marvel-nccr/ansible-role-bigdft/releases)

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

## Development and testing

This role uses [Molecule](https://molecule.readthedocs.io/en/latest/#) and [Docker](https://www.docker.com/) for tests.

After installing [Docker](https://www.docker.com/):

Clone the repository into a package named `marvel-nccr.bigdft` (the folder must be named the same as the Ansible Galaxy name)

```bash
git clone https://github.com/marvel-nccr/ansible-role-bigdft marvel-nccr.bigdft
cd marvel-nccr.bigdft
```

Then run:

```bash
pip install -r requirements.txt  # Installs molecule
molecule test  # runs tests
```

or use tox (see `tox.ini`):

```bash
pip install tox
tox
```

## Code style

Code style is formatted and linted with [pre-commit](https://pre-commit.com/).

```bash
pip install pre-commit
pre-commit run -all
```

## Deployment

Deployment to Ansible Galaxy is automated *via* GitHub Actions.
Simply tag a release `vX.Y.Z` to initiate the CI and release workflow.
Note, the release will only complete if the CI tests pass.

## License

MIT

BigDFT code is licensed under GNU GPL v2

## Contact

Please direct inquiries regarding Quantum Mobile and associated ansible roles to the [AiiDA mailinglist](http://www.aiida.net/mailing-list/).
