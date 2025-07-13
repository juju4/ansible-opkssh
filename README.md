# opkssh ansible role

[![Actions Status - Main](https://github.com/juju4/ansible-opkssh/workflows/AnsibleCI/badge.svg)](https://github.com/juju4/ansible-opkssh/actions?query=branch%3Amain)
[![Actions Status - Devel](https://github.com/juju4/ansible-opkssh/workflows/AnsibleCI/badge.svg?branch=devel)](https://github.com/juju4/ansible-opkssh/actions?query=branch%3Adevel)

Setup [opkssh](https://github.com/openpubkey/opkssh), OpenPubkey SSH on server.

See also
* https://blog.cloudflare.com/open-sourcing-openpubkey-ssh-opkssh-integrating-single-sign-on-with-ssh/

## Requirements & Dependencies

### Ansible

It was tested on the following versions:
 * 2.18

### Operating systems

Tested on Ubuntu 24.04, 22.04, Centos/Rockylinux 9.

## Example Playbook

Just include this role in your list.
For example

```yaml
- host: myhost
  roles:
    - juju4.opkssh
```

you probably want to review variables

## Variables

TBD

## Continuous integration

```
$ pip install molecule docker
$ molecule test
$ MOLECULE_DISTRO=ubuntu:24.04 molecule test --destroy=never
```

## Troubleshooting & Known issues

TBD

## License

BSD 2-clause
