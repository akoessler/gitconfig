# Global git config

Global git configuration files, shared across multiple machines (work, private) and environments (Windows, WSL).

## Usage

Checkout repository to ~/git

```
gh repo clone akoessler/gitconfig git
```

Link to the config in `~/git` in global user config `~/.gitconfig`, e.g.:

```
[include]
    path = ~/git/gitconfig-global.gitconfig
    path = ~/git/gitconfig-work.gitconfig
```

=> Global git config will be taken from the shared config in the repo.

Add more machine specific configuration here in this file.

## Linux / WSL

Note for Linux/WSL: The ssh and gpg config is made to make it work on Windows. For Linux and WSL the ssh and gpg commands must be reset:
```
[core]
    sshCommand = ssh
[gpg]
    program = gpg
```
