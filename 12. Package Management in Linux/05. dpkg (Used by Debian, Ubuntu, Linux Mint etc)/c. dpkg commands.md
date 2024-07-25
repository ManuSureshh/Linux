## DPKG Commands

### Basic DPKG Commands

| Command                                | Description                               |
|----------------------------------------|-------------------------------------------|
| `dpkg -i package.deb`                  | Install a package                         |
| `dpkg -r package_name`                 | Remove a package                          |
| `dpkg -P package_name`                 | Purge a package (remove with config files)|
| `dpkg -l`                              | List all installed packages               |
| `dpkg -L package_name`                 | List files installed by a package         |

### Query Options

| Command                                | Description                               |
|----------------------------------------|-------------------------------------------|
| `dpkg -s package_name`                 | Display package status                    |
| `dpkg -p package_name`                 | Display package information               |
| `dpkg -c package.deb`                  | List contents of a package file           |
| `dpkg -S /path/to/file`                | Find which package owns a file            |

### Additional Commands

| Command                                | Description                               |
|----------------------------------------|-------------------------------------------|
| `dpkg --configure -a`                  | Reconfigure unpacked packages             |
| `dpkg --audit`                         | Search for partially installed packages   |
| `dpkg-reconfigure package_name`        | Reconfigure an installed package          |
| `dpkg-deb --build directory`           | Create a package from a directory         |

### Examples of Combined Options

| Command                                | Description                               |
|----------------------------------------|-------------------------------------------|
| `dpkg -i --force-depends package.deb`  | Install, ignoring dependency issues       |
| `dpkg -r --force-all package_name`     | Forcefully remove a package               |
| `dpkg -i http://example.com/package.deb`| Install from URL                         |
