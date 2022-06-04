# Global git config

Global git configuration files, shared across multiple machines (work, private) and environments (Windows, WSL).

## Usage

Checkout repository to ~/git

Link to the config in `~/git` in global user config `~/.gitconfig`, e.g.:

```
[include]
    path = ~/git/gitconfig-global.gitconfig
    path = ~/git/gitconfig-work.gitconfig
```

=> Global git config will be taken from the shared config in the repo.

Add more machine specific configuration here in this file.
