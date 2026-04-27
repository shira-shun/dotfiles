# Raycast

This directory stores Raycast settings exports.

## Backup

1. Open Raycast.
2. Run `Export Settings & Data`.
3. Save the exported `.rayconfig` file to `~/Downloads`.
4. Run:

   ```sh
   ./raycast/bin/save-latest-export
   ```

The script copies the newest `~/Downloads/*.rayconfig` file into the chezmoi source state:

```text
home/dot_config/raycast/exports/current.rayconfig
```

## Restore

1. Open Raycast.
2. Run `Import Settings & Data`.
3. Select `~/.config/raycast/exports/current.rayconfig` after running `chezmoi apply`.

## Notes

- Keep the Raycast export encrypted with an export password before committing it.
- Do not commit decrypted JSON exports or local Raycast application data.
- Raycast's own export does not include everything, such as clipboard history.
