# Obsidian

- [Obsidian](https://obsidian.md) / [Help](https://help.obsidian.md/Home)

> [!bug] Conflicting shortcuts
> Obsidian confuses <kbd>fn</kbd> + <kbd>control</kbd> + <kbd>left</kbd> / <kbd>right</kbd> (the default [Mac window tiling shortcuts](https://support.apple.com/en-au/guide/mac-help/mchl9674d0b0/mac)) with <kbd>fn</kbd> + <kbd>left</kbd> / <kbd>right</kbd> (the [Windows keys on a Mac keyboard](https://support.apple.com/en-au/guide/mac-help/cpmh0152/mac) for <kbd>Home</kbd> / <kbd>End</kbd>). Forum post: [Obsidian confuses Mac window tiling shortcut for Windows Home/End shortcut](https://forum.obsidian.md/t/obsidian-confuses-mac-window-tiling-shortcut-for-windows-home-end-shortcut/91551).

- [ ] Make “readable” column width a bit wider
- [ ] Write a CSS snippet to format tables a bit nicer, using underlying theme names for colours
- [ ] Remove light borders from Catppuccin themes
- [ ] Update keyboard shortcuts snippet to work in reading mode
- [ ] Write a CSS snippet for advanced checklists
- [ ] Finish basic configuration settings below

## Settings

- Community plugins
	- *Turn on community plugins*
	- Install **Style Settings** plugin
- Appearance
	- Install **Catppuccin** theme
	- Font
		- Text font: **Fira Sans**
		- Monospace font: **FiraCode Nerd Font Mono**
	- Interface
		- Show inline title **OFF**
		- Show tab title bar **OFF**
		- Show ribbon **OFF**
	- Advanced
		- Native menus **OFF**
- Core plugins
	- Slash commands **ON**
	- 
- Update  [[#Hotkeys]]
- Add [[#CSS snippets]]
## Hotkeys

| Hotkey                                               | Unassign                | Assign                          |
| ---------------------------------------------------- | ----------------------- | ------------------------------- |
| <kbd>command</kbd> <kbd>1</kbd> through <kbd>8</kbd> | Go to tab #1 through #8 | Set as heading 1 through 6      |
| <kbd>command</kbd> <kbd>shift</kbd> <kbd>/</kbd>     |                         | Toggle Live Preview/Source mode |
| <kbd>command</kbd> <kbd>shift</kbd> <kbd>B</kbd>     |                         | Toggle left sidebar             |

## CSS snippets

Add snippets to `.obsidian/snippets` in a vault.

```css
/*
 .obsidian/snippets/kbd.css
 Style for <kbd> elements.
 Currently works in editing view only.
 */
.cm-html-embed kbd,
.table-cell-wrapper kbd {
    display: inline-block;
    color: var(--text-normal);
    padding: 0em 0.5em;
    border-radius: 0.2em;
    box-shadow: 0em 0.1em 0em var(--text-normal);
    border: 1px solid var(--text-normal);
    background-color: var(--background-primary);
}
```

```css
/* indentation.css
   Book style paragraph indentation.
   Designed to work with Minimal theme. */
[class="cm-line"]:not(:has(> br:only-child)) + [class="cm-line"],
[class="cm-line"]:not(:has(> br:only-child)) + [class="cm-active cm-line"],
[class="cm-active cm-line"]:not(:has(> br:only-child)) + [class="cm-line"],
[class="cm-active cm-line"]:not(:has(> br:only-child)) + [class="cm-active cm-line"] {
    text-indent: 2em;
}
```
