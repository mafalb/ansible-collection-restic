# Ansible Role - mafalb.restic.job

Configure a backup job.

## Basic Usage

```yaml
- name: Backup the whole system
  hosts: localhost
  roles:
  - role: mafalb.restic.install
  - role: mafalb.restic.repo
    repo: default
  - role: mafalb.restic.job
    job: wholesystem
    repo: default
    paths:
    - /
```

## Variables

```yaml
job: wholesystem
```

Name of the job.

---

```yaml
repo: system
```

Name of the repo used. The repo has to be present, use mafalb.restic.repo for this.

---

```yaml
dest: /etc/cron.daily/backup
```

Target file for the backup script

---

```yaml
paths:
- list
- of
- directories
- and
- files
```

---

```yaml
exclude:
- additional
- directories
- and
- files
- to
- exclude
```

The files in ```global_exclude``` are also excluded automatically. Use the ```exclude``` variable to extend ```global_exclude```.

## License

GPLv3

