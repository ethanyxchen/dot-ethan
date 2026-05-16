# chezmoi dotfiles

Manage this repository with [chezmoi](https://www.chezmoi.io/).

## Install chezmoi (Homebrew)

```bash
brew update
brew install chezmoi
```

Verify installation:

```bash
chezmoi --version
```

## Initialize and apply this repo

Replace `<repo-url>` with your repository URL.

```bash
chezmoi init <repo-url>
chezmoi apply
```

## Basic commands

Show pending changes:

```bash
chezmoi diff
```

Edit a managed file:

```bash
chezmoi edit ~/.zshrc
```

Preview what apply would change:

```bash
chezmoi apply --dry-run --verbose
```

Apply changes:

```bash
chezmoi apply
```

Add an existing file into source state:

```bash
chezmoi add ~/.gitconfig
```

Update from remote and apply:

```bash
chezmoi update
```
