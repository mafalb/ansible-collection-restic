# Ansible Collection - mafalb.restic

|||
|---|---|
|master|![master branch](https://github.com/mafalb/ansible-collection-restic/workflows/CI/badge.svg?branch=master)|
|dev|![dev branch](https://github.com/mafalb/ansible-collection-restic/workflows/CI/badge.svg?branch=dev)|

## Roles

### [mafalb.restic.install](roles/install/README.md)

This role installs restic. See also related ![Restic installation documentation](https://restic.readthedocs.io/en/latest/020_installation.html)

### [mafalb.restic.pkg_mgr](roles/pkg_mgr/README.md)

This role configures the package manager.

### [mafalb.restic.repo](roles/repo/README.md)

Configure a restic repo at the client. This does not initialize restic repositories, it just configures the machine to use one.

### [mafalb.restic.job](roles/job/README.md)

For scheduling a job.

## LICENSE

GPL Version 3
