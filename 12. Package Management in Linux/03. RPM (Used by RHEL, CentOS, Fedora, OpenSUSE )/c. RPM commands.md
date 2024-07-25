# RPM Commands

This document provides a comprehensive list of RPM (Red Hat Package Manager) commands along with their usage.

## Basic RPM Commands

| Command                                | Description                               |
|----------------------------------------|-------------------------------------------|
|``` rpm -ivh package.rpm ```                 | Install a package                         |
| `rpm -Uvh package.rpm`                 | Upgrade a package                         |
| `rpm -Fvh package.rpm`                 | Freshen a package (upgrade if installed)  |
| `rpm -e package_name`                  | Erase (remove) a package                  |
| `rpm -q package_name`                  | Query a package                           |

## Query Options

| Command                                | Description                               |
|----------------------------------------|-------------------------------------------|
| `rpm -qa`                              | Query all installed packages              |
| `rpm -qf /path/to/file`                | Query a package file                      |
| `rpm -qi package_name`                 | Query a package for detailed information  |
| `rpm -ql package_name`                 | Query a package for a list of files       |
| `rpm -qd package_name`                 | Query a package for documentation files   |
| `rpm -qc package_name`                 | Query a package for configuration files   |
| `rpm -qR package_name`                 | Query a package for dependencies          |
| `rpm -q --whatprovides /path/to/file`  | Query what package owns a file            |
| `rpm -q --whatprovides capability`     | Query for packages providing a capability |

## Verification Commands

| Command                                | Description                               |
|----------------------------------------|-------------------------------------------|
| `rpm -V package_name`                  | Verify a package                          |
| `rpm -Va`                              | Verify all packages                       |
| `rpm -Vp package.rpm`                  | Verify a package file                     |

## Additional Commands

| Command                                | Description                               |
|----------------------------------------|-------------------------------------------|
| `rpm -q --changelog package_name`      | Show RPM package changelog                |
| `rpm -q --provides package_name`       | Show package provides                     |
| `rpm -q --requires package_name`       | Show package dependencies                 |
| `rpm --rebuilddb`                      | Rebuild RPM database                      |
| `rpm --import /path/to/key`            | Import a GPG key                          |
| `rpm -q --dbpath`                      | Show the RPM database info                |
| `rpmbuild -ba package.spec`            | Build a package from a spec file          |

## Examples of Combined Options

| Command                                | Description                               |
|----------------------------------------|-------------------------------------------|
| `rpm -Uvh --replacepkgs package.rpm`   | Install and replace any older versions    |
| `rpm -ivh --nodeps package.rpm`        | Install without checking dependencies     |
| `rpm -Uvh --nodeps package.rpm`        | Upgrade without checking dependencies     |
| `rpm -ivh http://example.com/package.rpm` | Install from URL                        |
