# Changelog

## 0.0.5 XXXX-XX-XX

### Changes to CI

- use actions/checkout@v2
- use default working-dir

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
