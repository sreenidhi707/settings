# `git`

| Command | Description |
| ------- | ----------- |
| `git diff > changes.patch`           | Save **uncommitted** changes into a patch |
| `git diff -- cached > changes.patch` | Save **committed** changes into a patch   |
| `git apply changes.patch` | Apply patch |
| `git checkout -- .`                  | Revert all unstaged changes in current working directory |
| `git checkout -- path/to/file/to/revert` | Revert a single file, which was not committed |
| `git mv old_name new_name` | Rename a file, `old_name` to `new_name` |
| `git rm file_name` | Delete a file |
| `git rm -r folder_name` | Delete a folder from git and filesystem |
| `git rm -r --cached folder_name` | Delete a folder from git but not from filesystem |
| `git log --grep=<pattern>` | `grep` in commit messages |


### `commit`
| Command | Description |
| ------- | ----------- |
| `git commit -m "new message"`           | Commit files that have already been added to the staging area |

### `stash`
| Command | Description |
| ------- | ----------- |
| `git stash list`                           | List all stashes |
| `git stash push -m "stash-name"`           | Creates a named stash called 'stash-name' |
| `git stash push file1.cpp file2.cpp`       | Stash specific files |
| `git stash push -p -m "stash-name"`        | Allows you to stash portions of the changes, like a single file, it asks for what to do for each hunk |
| `git stash apply`                          | Applies the stash in top of stack |
| `git stash apply <index>`                  | Applies the stash at <index> |
| `git stash drop`                           | Drop the stash in top of stack |
| `git stash show`                              | Shows the summary of the changes at the top of stash |
| `git stash show -p`                           | Shows the diff of the changes at the top of stash |
| `git stash show stash@{n}`                    | Shows the summary of the changes at index `n` of stash |
| `git stash show stash@{n} -p`                 | Shows the diff of the changes at index `n` of stash |

### `push`
| Command | Description |
| ------- | ----------- |
| `git diff --stat --cached origin/master`           | Shows the list of files that will be pushed to `origin/master` |
| `git diff --stat --cached origin/branch_name`           | Shows the list of files that will be pushed to `origin/branch_name` |

