## v1.2.0

### Fix
* Replace flatten jinja filter with **list**.
* Call module with FQCN.

### Enhancements
* Use comment jinja filter with ansible_managed to allow multi-lines comment.

## v1.1.2

### Enhancements
* Use to_nice_json to manage packages list.

## v1.1.1

### Fix
* Set empty dependencies line to fix Galaxy warning.
* Fix small warnings from linter.
* Fix E405 Remote package tasks should have a retry.

## v1.1.0

### Fix
* Ensure to keep permissions for configuration files.

### Enhancements
* Allow possibility to add symlinks in Xymon configuration.

## v1.0.0

### Features
* Install `xymon` packages for Debian based distros.
* Manage `xymon` server configuration (/etc).
* Ensure to restart `xymon` server service if configuration changed.
* Ensure `xymon` server service is enabled and started.
