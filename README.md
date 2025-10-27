# Gitsync.sh

A simple script to auto sync a list of git directories.

# Usage

1. Clone repo and copy the script in your script dir.

```bash
git clone https://github.com/trgr-boi/gitsync.sh && cp gitsync.sh/gitsync ~/.local/bin/
```

2. Add directories and groups.

- You first need to add a group, or add to the already existing groups.
- To add a new directory to a existing group, just add a new line in the group list and add `"path/to/dir"`
- To add a new group, make a new list like this:

  ```bash
  NEW_GROUP_DIR=(
    "path/to/dir"
  )
  ```

- And add it to the `ALL_DIRS` variable:
  ```bash
  ALL_DIRS=("${NOTES_DIRS[@]}" "${DOTFILES_DIRS[@]}" "${NEW_GROUP_DIR[@]}")
  ```

3. Use with `gitsync {pull|push} {group}`

## Guideline

- When you start editing: `gitsync pull {group}`
- when you are finished: `gitsync push {group}`

## Todo

- [x] add a way to pull
- [x] parameter option for `pull` or `push`
- [x] select what you want to sync (groups?)
