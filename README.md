# git config extending

A place for me to put extended git configuration options

## How to use

- Clone this repository
- Add this to your global (or local) git configuration (~/.gitconfig)

```bash

# include configuration if under specific directory
# line 1 is the directory where this configuration will be included
# line 2 is the path to the configuration
[includeIf "gitdir:~/projects/"]
    path = ~/projects/git-config/.gitconfig.aliases
```

### Updating .gitconfig easier

To make it easier to modify the `.gitconfig` if needed, you create a symbolic link to the global config

```bash
  # modify this if you have the project under a different directory
  ln -s ~/.gitconfig ~/projects/git-config/.gitconfig
```

### Personal directory

A personal directory exists in this project to dump things that shouldn't be in source control
