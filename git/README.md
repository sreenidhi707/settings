# `git`

| Command | Description |
| ------- | ----------- |
| `git diff > changes.patch`           | Save **uncommitted** changes into a patch |
| `git diff -- cached > changes.patch` | Save **committed** changes into a patch   |
| `git apply changes.patch` | Apply patch |
| `git checkout -- .`                  | Revert all unstaged changes in current working directory |
| `git checkout -- path/to/file/to/revert` | Revert a single file, which was not committed |

### `commit`
| Command | Description |
| ------- | ----------- |
| `git commit -m "new message"`           | Commit files that have already been added to the staging area |
