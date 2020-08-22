# Ansible Role - mafalb.restic.install

This role installs restic

## Basic Usage

```yaml
- name: install restic
  hosts: localhost
  roles:
  - role: mafalb.restic.install
```

## Variables

```exclude_global``` optional variable with a list of paths to be excluded, sensitive defaults are provided. These paths are always excluded. You can specify another set of exclude paths per job (see mafalb.restic.job)

```yaml
exclude_global:
- /dev
- /dev/shm
- /proc
- /run
- /sys
- /var/cache/fscache
- /var/cache/yum
```

## License

GPLv3
