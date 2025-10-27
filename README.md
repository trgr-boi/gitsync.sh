# Gitsync.sh

A simple script to auto sync a list of git directories.

# Usage

1. Clone repo and copy the script in your script dir.

```bash
git clone https://github.com/trgr-boi/gitsync.sh && cp gitsync.sh/gitsync ~/.local/bin/
```

2. Add your dirs in the `REPO_DIRS` list.

```bash
REPO_DIRS(
  "$HOME/Notes"
  "$HOME/Projects"
  "..."
)
```

3. Use with `gitsync`
