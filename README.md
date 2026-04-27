# dotfiles

Personal dotfiles and app settings.

## chezmoi

This repository uses chezmoi with `home/` as the source root.

Use this checkout as the chezmoi source:

```sh
chezmoi init --source "$(pwd)"
```

Preview changes:

```sh
chezmoi --source "$(pwd)" diff
```

Apply changes:

```sh
chezmoi --source "$(pwd)" apply
```

## Raycast

Raycast settings are managed in [`raycast/`](./raycast/).
