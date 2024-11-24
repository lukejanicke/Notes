# Zed

- [Zed](https://zed.dev) / [Documentation](https://zed.dev/docs/)

## Installation

Download and install **Zed** directly from the official website.

## CLI

To install the **Zed CLI**, you can either:

- Go to the main menu and select **Zed → Install CLI**.
- Use the command palette by pressing <kbd>Command</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd> and typing `cli: install`.

## Settings

> [!bug] Inconsistent font sizing
> It is not possible to set UI and buffer font sizes accurately.

```json
// ~/.config/zed/settings/json
// Run `zed: open default settings` to see Zed's default settings

{
  // Assistant configuration is changed by client.
  "assistant": {
    "default_model": {
      "provider": "copilot_chat",
      "model": "gpt-4o"
    },
    "version": "2"
  },
  "base_keymap": "VSCode", // This is default but I want to lock it in.
  "ui_font_family": "Fira Sans",
  "ui_font_fallbacks": ["Zed Plex Sans"],
  "buffer_font_family": "Fira Code",
  "buffer_font_fallbacks": ["FiraCode Nerd Font Mono"],
  "theme": {
    "mode": "system",
    "light": "Catppuccin Latte",
    "dark": "Catppuccin Mocha"
  }
}

```