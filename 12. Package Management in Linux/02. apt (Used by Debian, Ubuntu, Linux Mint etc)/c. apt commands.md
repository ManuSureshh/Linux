## APT Commands

### Basic APT Commands

| Command                                | Description                               |
|----------------------------------------|-------------------------------------------|
| `apt install package`                  | Install a package                         |
| `apt remove package`                   | Remove a package                          |
| `apt purge package`                    | Purge a package (remove with config files)|
| `apt update`                           | Update package lists                      |
| `apt upgrade`                          | Upgrade all packages                      |

### Query Options

| Command                                | Description                               |
|----------------------------------------|-------------------------------------------|
| `apt list --installed`                 | List all installed packages               |
| `apt search keyword`                   | Search for a package                      |
| `apt show package`                     | Display information about a package       |
| `apt policy package`                   | Show package version and repository info  |

### Advanced Commands

| Command                                | Description                               |
|----------------------------------------|-------------------------------------------|
| `apt full-upgrade`                     | Upgrade all packages, remove obsoletes    |
| `apt autoremove`                       | Remove unused packages                    |
| `apt clean`                            | Clean the local repository cache          |
| `apt edit-sources`                     | Edit the sources.list file                |

### Examples of Combined Options

| Command                                | Description                               |
|----------------------------------------|-------------------------------------------|
| `apt install package -y`               | Install a package without prompting       |
| `apt upgrade --with-new-pkgs`          | Upgrade, allowing new dependencies        |
| `apt install package --no-install-recommends` | Install without recommended packages |
| `apt install http://example.com/package.deb` | Install from URL                        |
