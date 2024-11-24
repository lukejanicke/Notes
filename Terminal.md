# Terminal

- [Terminal User Guide](https://support.apple.com/en-au/guide/terminal/welcome/mac) / [Keyboard shortcuts](https://support.apple.com/en-au/guide/terminal/trmlshtcts/mac)
- [Catppuccin (GitHub)](https://github.com/catppuccin/Terminal.app)

See [[Shell Shortcuts]] for **Terminal** and other shell keyboard shortcuts.

> [!note] [[Fish]] sets **Terminal** window and tab bar titles
> [[Fish]] sets **Terminal** window and tab bar titles to an abbreviated current working directory, and prepends the shell name if the default shell is left. For example, `zsh ~/D/Python`. Changing directory when not in [[Fish]] shell will not update window and tab bars. I would prefer that **Terminal** settings take precedence.

## Settings

Hide login information.

```zsh
touch .hushlogin
```

From the **View**, select **Hide Marks**.

Make sure **FiraCode Nerd Font Mono** is installed.

Remove default profiles.

Import modified **Catppuccin** profiles.

For new profiles, change the following settings.

- Text
	- Font: **FiraCode Nerd Font Mono 13**
- Window
	- Title: **Terminal**
	- Select **Working directory or arguments**, **Path**
	- Select **Shell command name**
	- Deselect **Active process name**, **Arguments** 
	- Deselect **Dimensions**
	- Window Size, Columns: **90**, Rows: **30**
	- Deselect **Restore text when reopening windows**
- Tab
	- Select **Working directory or document**, **Path**
	- Deselect **Active process name** and **Arguments**
- Keyboard
	- Select **Use Option as Meta key**. (*See [Shortcuts](#Shortcuts) below.*)
- Advanced
	- Select **Set locale environment variables on startup** (*Required for `en_AU.UTF-8` locale.*)
