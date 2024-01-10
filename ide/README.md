
## `vi`

| Command | Description |
| ------- | ----------- |
| `^` | Goto first non-blank character in line |
| `SHIFT D` | Deletes from current cursor position to end of current line |

## `vscode`
| Command | Description |
| ------- | ----------- |
| `⌘K ⌘S` | Show keyboard shortcuts |
| `code folding`  |                    |
| `⌘K 0` | Fold all regions in file   |
| `⌘K j` | Unfold all regions in file |
| `⌘K ⌘[` | Fold all subregions |
| `⌘K ⌘]` | Unfold all subregions |

Using vscode to debug python code
Sometimes you may encounter 'module not found' error, when using the debugger of vscode, even though you might have pip installed the package. You may have to install the package using the python binary which is used by the vscode debugger. Run the command below

`venv/bin/python -m pip install scikit-image`

where `venv/bin/python` is the path of the python which is used by vscode debugger and `scikit-image` is the missing package name.
### Snippet to insert timestamp in markdown documents
- Open Command Palette
- Select "Preferences: Configure User Snippets"
- Select "markdown.json"
- Insert this
  ```
    "Insert Timestamp": {
    "prefix": "insts",
    "body": [
        "$CURRENT_YEAR-$CURRENT_MONTH-${CURRENT_DATE}_${CURRENT_HOUR}h:${CURRENT_MINUTE}m:${CURRENT_SECOND}s"
    ],
    "description": "Insert timestamp"
  }
  ```
## `comparison`
|  Command group  |       Command                  |    vi                  |    emacs    | vscode     |
| ----------------| -----------                    | -------                | ----------- |----------- |
| `navigation`    |                                |                        |             |
|                 | Goto top of file               |   `gg`                 |             |  `⌘`:arrow_up:    |
|                 | Goto end of file               |   <kbd>Shift</kbd>`G`  |             |  `⌘`:arrow_down:    |
|                 | Page UP                        |   <kbd>Ctrl</kbd>`b`   |             |   <kbd>Page UP</kbd>   |
|                 | Page DOWN                      |   <kbd>Ctrl</kbd>`f`   |             |   <kbd>Page DOWN</kbd>   |
|                 | Goto beginning of line         |   `0` OR `^`           |             |  `⌘`:arrow_left:    |
|                 | Goto end of line               |   `$`                  |             |  `⌘`:arrow_right:    |
|                 | Go one word forward            |   `w`           |                    |      |
|                 | Go one word backward           |   `b`                  |             |     |
|                 | Go back to previous location   |   <kbd>Ctrl</kbd> `o`  |             |  <kbd>Ctrl</kbd> `-`    |
|                 | Go forward to next location    |   <kbd>Ctrl</kbd> `i`  |             | <kbd>Ctrl</kbd> <kbd>Shift</kbd> `-`    |
| `code folding`  |                    |
| `⌘K 0` | Fold all regions in file   |
| `⌘K j` | Unfold all regions in file |
| `⌘K ⌘[` | Fold all subregions |
| `⌘K ⌘]` | Unfold all subregions |
| `copy`     |                          |         |
|                 | Copy current line               |   `yy`                 |             |       |
| `paste`     |                          |         |
|                 | Paste content in buffer               |   `p`                 |             |       |
| `deletions`     |                          |         |
|                 | Delete current line      |   `dd`  |             |  <kbd>Shift</kbd> `⌘k`  |
