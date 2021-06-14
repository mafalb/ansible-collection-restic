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

---

```yaml
cachedir: /var/cache/restic
```

---

```yaml
restic_repo_state: present
```

set to absent if you want to remove the repo

---

```yaml
restic_nice: ionice -c2 nice -n +19
```

not set per default. use this if you want to run your jobs with special nice or scheduling

---

```yaml
restic_repo_local_group: group
```

make it possible for members of group to access the repo password file. optional.

## License

GPLv3

