# Typst

- [Typst](https://typst.app/home/)
- [Tinymist](https://github.com/Myriad-Dreamin/tinymist) / [Documentation](https://myriad-dreamin.github.io/tinymist/)

## Installation

Install **Typst** with [Homebrew](Homebrew.md).

```zsh
brew install typst
```

## Usage

Compile `file.typ` to `file.pdf`.

```zsh
typst compile file.typ
```

Watch `file.typ` and recompile on save.

```zsh
typst watch file.typ
```

## Visual Studio Code

Install the **Tinymist** extension for Visual Studio Code.

### Tinymist settings

| Name                     | Setting    |
| ------------------------ | ---------- |
| Tinymist: Export PDF     | `onSave`   |
| Tinymist: Formatter Mode | `typstyle` |

Hide action Controls on the editor panel by adding the following to `settings.json`.

```JSON
"[typst]": {
	"editor.codeLens": false
}
```
