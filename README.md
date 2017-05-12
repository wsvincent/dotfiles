# Notorious dotfiles

## Installation

### Using Git and the bootstrap script

To update, `cd` into your local `dotfiles` repository and then, if using zsh, specify bash for command:

```bash
bash bootstrap.sh
```

### Add custom commands without creating a new fork

If `~/.extra` exists, it will be sourced along with the other files. You can use this to add a few custom commands without the need to fork this entire repository, or to add commands you don’t want to commit to a public repository.

### Sensible OS X defaults

When setting up a new Mac, you may want to set some sensible OS X defaults:

```bash
./.osx
```

### Install Homebrew formulae

When setting up a new Mac, you may want to install some common [Homebrew](http://brew.sh/) formulae (after installing Homebrew, of course):

```bash
./.brew
```

### Post-commit

```bash
ln -s ../../post-commit.sh .git/hooks/post-commit
```
