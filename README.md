## `disk usage`
```
$ du --help
Usage: du [OPTION]... [FILE]...
  or:  du [OPTION]... --files0-from=F
Summarize disk usage of the set of FILEs, recursively for directories.

Mandatory arguments to long options are mandatory for short options too.
  -0, --null            end each output line with NUL, not newline
  -a, --all             write counts for all files, not just directories
      --apparent-size   print apparent sizes, rather than disk usage; although
                          the apparent size is usually smaller, it may be
                          larger due to holes in ('sparse') files, internal
                          fragmentation, indirect blocks, and the like
  -B, --block-size=SIZE  scale sizes by SIZE before printing them; e.g.,
                           '-BM' prints sizes in units of 1,048,576 bytes;
                           see SIZE format below
  -b, --bytes           equivalent to '--apparent-size --block-size=1'
  -c, --total           produce a grand total
  -D, --dereference-args  dereference only symlinks that are listed on the
                          command line
  -d, --max-depth=N     print the total for a directory (or file, with --all)
                          only if it is N or fewer levels below the command
                          line argument;  --max-depth=0 is the same as
                          --summarize
      --files0-from=F   summarize disk usage of the
                          NUL-terminated file names specified in file F;
                          if F is -, then read names from standard input
  -H                    equivalent to --dereference-args (-D)
  -h, --human-readable  print sizes in human readable format (e.g., 1K 234M 2G)
      --inodes          list inode usage information instead of block usage
  -k                    like --block-size=1K
  -L, --dereference     dereference all symbolic links
  -l, --count-links     count sizes many times if hard linked
  -m                    like --block-size=1M
  -P, --no-dereference  don't follow any symbolic links (this is the default)
  -S, --separate-dirs   for directories do not include size of subdirectories
      --si              like -h, but use powers of 1000 not 1024
  -s, --summarize       display only a total for each argument
  -t, --threshold=SIZE  exclude entries smaller than SIZE if positive,
                          or entries greater than SIZE if negative
      --time            show time of the last modification of any file in the
                          directory, or any of its subdirectories
      --time=WORD       show time as WORD instead of modification time:
                          atime, access, use, ctime or status
      --time-style=STYLE  show times using STYLE, which can be:
                            full-iso, long-iso, iso, or +FORMAT;
                            FORMAT is interpreted like in 'date'
  -X, --exclude-from=FILE  exclude files that match any pattern in FILE
      --exclude=PATTERN    exclude files that match PATTERN
  -x, --one-file-system    skip directories on different file systems
      --help     display this help and exit
      --version  output version information and exit

Display values are in units of the first available SIZE from --block-size,
and the DU_BLOCK_SIZE, BLOCK_SIZE and BLOCKSIZE environment variables.
Otherwise, units default to 1024 bytes (or 512 if POSIXLY_CORRECT is set).

The SIZE argument is an integer and optional unit (example: 10K is 10*1024).
Units are K,M,G,T,P,E,Z,Y (powers of 1024) or KB,MB,... (powers of 1000).

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
Full documentation at: <http://www.gnu.org/software/coreutils/du>
or available locally via: info '(coreutils) du invocation'
```
| Command | Description |
| ------- | ----------- |
| `sudo du -sh ./* \| sort -hr` | disk usage summary of current folder in human readable format `\|` sort in reverse order and show output in human readable format |

## `docker`


## `grep`

| Command | Description |
| ------- | ----------- |
| `grep -r --include \*.py "search-term"` | grep inside all .py files recursively in a folder |

## `less`

| Command | Description |
| ------- | ----------- |
| `-N` | Show line numbers |
| `g` | Goto beginning of file |
| `G` | Goto end of file |
| `SPC` | Page down |
| `b` | Page up |
| `/<text>` | Search forwards |
| `?<text>` | Search backwards |
| `-S` | Disable line wrap, to see chopped portion press right arrow |
| `q` | Quit |

## `screen`

| Command | Description |
| ------- | ----------- |
| `screen -ls` | list all currently running `screen` sessions |
| `echo $STY` | show the name of current `screen` session, if attached |
| `screen -S <screen-name>` | Start a new `screen` session with name `screen-name` |
| `screen -r <screen-name>` | Attach to a running `screen` session with name `screen-name` |
| `screen -wipe` | remove dead `screen`s |
| `C-a d` | Detach  |

## `vi`

## `vscode`
| Command | Description |
| ------- | ----------- |
| `⌘K ⌘S` | Show keyboard shortcuts |
| `⌘K ⌘[` | Fold all subregions |
| `⌘K ⌘]` | Unfold all subregions |
