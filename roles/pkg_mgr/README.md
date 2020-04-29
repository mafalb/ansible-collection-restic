# Ansible Role - mafalb.restic.pkg_mgr

Ansible role mafalb.restic.pkg_mgr
Provides the dnf/yum/whatever repository for installing restic.

## Basic Usage

```yaml
- name: install repository for the package manager
  hosts: localhost
  roles:
  - role: mafalb.restic.pkg_mgr
```

## Variables

None

## License

GPLv3
