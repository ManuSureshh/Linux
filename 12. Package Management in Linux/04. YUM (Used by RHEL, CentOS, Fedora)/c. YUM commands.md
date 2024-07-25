
## YUM Commands

### Basic YUM Commands

| Command                                | Description                               |
|----------------------------------------|-------------------------------------------|
| `yum install package`                  | Install a package                         |
| `yum update package`                   | Update a package                          |
| `yum update`                           | Update all packages                       |
| `yum remove package`                   | Remove a package                          |
| `yum list installed`                   | List all installed packages               |

### Query Options

| Command                                | Description                               |
|----------------------------------------|-------------------------------------------|
| `yum list available`                   | List all available packages               |
| `yum search keyword`                   | Search for a package                      |
| `yum info package`                     | Display information about a package       |
| `yum provides /path/to/file`           | Find which package provides a file        |
| `yum deplist package`                  | Display dependencies of a package         |

### Group Commands

| Command                                | Description                               |
|----------------------------------------|-------------------------------------------|
| `yum grouplist`                        | List all available groups                 |
| `yum groupinstall 'Group Name'`        | Install a package group                   |
| `yum groupremove 'Group Name'`         | Remove a package group                    |
| `yum groupinfo 'Group Name'`           | Display information about a package group |

### Additional Commands

| Command                                | Description                               |
|----------------------------------------|-------------------------------------------|
| `yum clean all`                        | Clean all cached files                    |
| `yum repolist`                         | List all repositories                     |
| `yum history`                          | Display transaction history               |
| `yum check-update`                     | Check for available updates               |

### Examples of Combined Options

| Command                                | Description                               |
|----------------------------------------|-------------------------------------------|
| `yum install package --skip-broken`    | Install a package, skipping broken deps   |
| `yum update --security`                | Update only security packages             |
| `yum remove package --remove-leaves`   | Remove a package and its unused deps      |
| `yum install http://example.com/package.rpm` | Install from URL 
