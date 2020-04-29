# Ansible Role - mafalb.restic.repo

bla

## Basic Usage

```yaml
- name: install repo
  hosts: localhost
  roles:
  - role: mafalb.restic.repo
    repo: default
    url: sftp:host:/
```

## Variables

```yaml
repo: default
```

Name of the repository

---

```yaml
url: /path/to/repo
```

```yaml
url: sftp:sftp.example.com:/path/to/repo
```

etc... any valid URL to a restic repo is allowed, see the [documentation of restic](https://restic.readthedocs.io/en/latest/030_preparing_a_new_repo.html#)

## License

GPLv3

