# Changelog

## 0.3.0 2021-07-14

- support for Rocky 8
- support for Debian 9

## 0.2.0 2021-06-16

- add nice and renice option for repos
- add the possibility to add tags to jobs
- add the possibility to specify groupship of password file
- changes in CI

## 0.1.1 2020-12-09

### Changes

- fix loop warning - set loop_var

### Changes to CI

- do not run when pushing tags
- do not test on CentOS 6 anymore

## 0.1.0 2020-10-20

### Added

- added an absent state for job and repo
- set cachedir per repo (defaults to /var/cache/restic)
- more default global exclude paths
- you can inject additional arguments into the backup job script, e.g. -v
- check for / in excludes and remove ignore it silently

### Changes to CI

- use actions/checkout@v2
- use default working-dir
- update apt cache
- CI against ansible 2.9 and 2.10
- CI against Fedora 33

## 0.0.4 2020-08-25

### Changed

- fix executable bit for global exclude list
- exclude /selinux

### Changed in CI

- fix internal network definition in molecule
- do not force molecule 3.0.4 anymore

## v0.0.3 2020-08-22

### Added

- CHANGELOG

### Changed

- a lot of changes and bug fixes to CI
- explicitly set mode to make ansible-lint happy / CVE-2020-1736
- a lot of other changes

### Removed

- drop support for fedora 30 (EOL)
