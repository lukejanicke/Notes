# Node

- [Node.js](https://nodejs.org/en/)
- [Installing Node.js via package managers: nvm](https://nodejs.org/en/download/package-manager/all#nvm)
- [nvm-sh](https://github.com/nvm-sh) / [nvm](https://github.com/nvm-sh/nvm)

## Installation

Install **nvn**.

```zsh
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.1/install.sh | bash
```

Copy the following to `~/.zshrc`.

```zsh
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"
```

Close and restart Terminal or `source ~/.zshrc`.

Verify the installation.

```zsh
nvm -v
```

Install the latest version of Node.

```zsh
nvm install node
```

Verify the installation.

```zsh
node -v
```

## npx

Use `npx <package>` to run packages whether they are local, global, or even not installed.
