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

### `stash`
| Command | Description |
| ------- | ----------- |
| `git stash list`                           | List all stashes |
| `git stash push -m "stash-name"`           | Creates a named stash called 'stash-name' |

### `push`
| Command | Description |
| ------- | ----------- |
| `git diff --stat --cached origin/master`           | Shows the list of files that will be pushed to `origin/master` |
| `git diff --stat --cached origin/branch_name`           | Shows the list of files that will be pushed to `origin/branch_name` |

