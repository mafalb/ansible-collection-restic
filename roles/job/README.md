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
restic_job_state: present
```

set to absent if you want to remove the job

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

---

```yaml
restic_nice: ionice -c2 nice -n +19
```

not set per default. use this if you want to run your jobs with special nice or scheduling

## License

GPLv3