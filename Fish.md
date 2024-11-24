# Fish

- [Fish](https://fishshell.com) / [Documentation](https://fishshell.com/docs/current/index.html)
	- [Fish for bash users](https://fishshell.com/docs/current/fish_for_bash_users.html)
	- [Writing your own prompt](https://fishshell.com/docs/current/prompt.html)
- [Catppuccin (GitHub)](https://github.com/catppuccin/fish)

## Installation

Install **Fish** with [[Homebrew]].

```shell
brew install fish
```

Make **Fish** the default shell.

```shell
sudo dscl . -create /Users/$(whoami) UserShell /opt/homebrew/bin/fish
```

Restore [[Zsh]] as the default shell with:

```shell
sudo dscl . -create /Users/$(whoami) UserShell /bin/zsh
```

Confirm which shell is default with:

```shell
dscl . -read /Users/$(whoami) UserShell
```

## Configuration

Configure **Fish** from `~/.config/fish/config.fish`.

Get custom configuration from [dotfiles](https://github.com/lukejanicke/dotfiles).

```shell
wget -P ~/.config/fish https://raw.githubusercontent.com/lukejanicke/dotfiles/master/.config/fish/config.fish
```

## Catppuccin

[dotfiles](https://github.com/lukejanicke/dotfiles) includes Catppuccin theme files and [[Zsh]] and [[Fish]] configuration.

Install **Catppuccin** theme for **Fish** manually.

Create the **Fish** themes directory.

```shell
mkdir ~/.config/fish/themes/
```

Copy **Catppuccin** theme files from the repository into the **Fish** themes directory.

```shell
wget -P ~/.config/fish/themes https://raw.githubusercontent.com/catppuccin/fish/main/themes/Catppuccin%20Latte.theme
wget -P ~/.config/fish/themes https://raw.githubusercontent.com/catppuccin/fish/main/themes/Catppuccin%20Frappe.theme
wget -P ~/.config/fish/themes https://raw.githubusercontent.com/catppuccin/fish/main/themes/Catppuccin%20Macchiato.theme
wget -P ~/.config/fish/themes https://raw.githubusercontent.com/catppuccin/fish/main/themes/Catppuccin%20Mocha.theme
```

## Help

| Command          | Description                                                     |
| ---------------- | --------------------------------------------------------------- |
| `help`           | Open online help documentation.                                 |
| `help [command]` | Open online help documentation for a specific command.          |
| `man [command]`  | Display the manual page for a specific command in the terminal. |
