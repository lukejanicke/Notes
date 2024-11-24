# zoxide

- [zoxide (GitHub)](https://github.com/ajeetdsouza/zoxide)

# Installation

Install **zoxide** with [[Homebrew]].

```shell
brew install zoxide
```

For [[Zsh]], add the following to `~/.zshrc`.

```shell
eval "$(zoxide init zsh)"
alias cd="z"
```

For [[Fish]], add the following to `~/.config/fish/config.fish`.

```shell
zoxide init fish | source
alias cd='z'
```
