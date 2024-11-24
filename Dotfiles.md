# Dotfiles

- [Dotfiles (GitHub)](https://github.com/lukejanicke/dotfiles)

## Setup

Create a bare repository in `~/Documents`.

```shell
git init --bare ~/Documents/Dotfiles
```

Create an alias in `.zshrc` or `~/.config/fish/fish.config`.

```shell
alias dotfiles='/usr/bin/git --git-dir=$HOME/Documents/Dotfiles --work-tree=$HOME'
```

Set the repository to not show untracked files.

```shell
dotfiles config --local status.showUntrackedFiles no
```

Add dotfiles to the repository and commit.

```shell
dotfiles add .zshrc
dotfiles commit -m "Let there be dotfiles\"
```

Create a repository on GitHub ([lukejanicke](https://github.com/lukejanicke)/[dotfiles](https://github.com/lukejanicke/dotfiles)).

Add the remote repository to the bare repository.

```shell
dotfiles remote add origin git@github.com:lukejanicke/dotfiles.git
```

Push changes.

```shell
dotfiles push -u origin master
```
