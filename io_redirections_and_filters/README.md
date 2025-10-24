# Project 2: Shell, I/O Redirections and Filters

## Description
This project practices Unix **redirections**, **pipes**, and **text filters**. You will learn to chain commands with `|`, redirect STDIN/STDOUT/STDERR, manipulate files and streams, and use common text-processing tools (`head`, `tail`, `find`, `wc`, `sort`, `uniq`, `grep`, `tr`, `rev`, `cut`). Scripts are intentionally minimal and follow strict formatting rules.

## Learning Objectives
By the end of this project, you should be able to explain:
- Standard streams (STDIN/STDOUT/STDERR) and how to redirect them (`>`, `>>`, `<`, `2>`, `&>`)
- How to send output of one program to another program’s input using **pipes** (`|`)
- What special characters do: whitespace, quotes (single/double), backslash, `#`, `|`, `;`, `~`
- Core filters: `head`, `tail`, `find`, `wc`, `sort`, `uniq`, `grep`/patterns, `tr`, `rev`, `cut`
- How to combine filters + redirections to solve tasks
- The purpose and format of `/etc/passwd` and `/etc/shadow` (read-only, for parsing)

## Requirements
- Allowed editors: `vi`, `vim`, `emacs`
- Environment: Ubuntu **20.04 LTS**
- **All scripts must be exactly two lines long** (`wc -l file` → `2`)
- All files must end with a new line
- The first line of every file must be exactly `#!/bin/bash`
- A `README.md` at the root of this project describing what each script does
- **Do not** use backticks, `&&`, `||`, or `;`
- **Do not** use `sed` or `awk`
- All scripts must be executable (`chmod u+x <file>`)

## Files

| File | Description |
|------|-------------|
| `0-hello_world` | Prints `Hello, World` to standard output. |
| `1-confused_smiley` | Displays a confused smiley: `"(Ôo)'`. |
| `2-hellofile` | Displays the content of `/etc/passwd`. |
| `3-twofiles` | Displays the content of `/etc/passwd` **and** `/etc/hosts`. |
| `4-lastlines` | Displays the **last 10 lines** of `/etc/passwd`. |
| `5-firstlines` | Displays the **first 10 lines** of `/etc/passwd`. |
| `6-third_line` | Displays the **3rd line** of the file `iacta` (from CWD). No `sed`. |
| `7-file` | Creates a file named `\*\\'"Best School"\'\\*$\?\*\*\*\*\*:)` containing `Best School` + newline. |
| `8-cwd_state` | Writes the result of `ls -la` into `ls_cwd_content` (overwrite or create). |
| `9-duplicate_last_line` | Duplicates the **last line** of `iacta`. |
| `10-no_more_js` | Deletes all regular `*.js` files in CWD and **subdirectories**. |
| `11-directories` | Counts the number of directories and subdirectories in CWD (exclude `.` and `..`, include hidden). |
| `12-newest_files` | Displays the **10 newest** files in CWD (one per line, newest first). |
| `13-unique` | Prints only words that appear **exactly once** from STDIN; output sorted, one per line. |
| `14-findthatword` | Displays lines containing `root` from `/etc/passwd`. |
| `15-countthatword` | Displays the **number of lines** containing `bin` in `/etc/passwd`. |
| `16-whatsnext` | Displays lines containing `root` and the **3 following lines** from `/etc/passwd`. |
| `17-hidethisword` | Displays all lines in `/etc/passwd` **not** containing `bin`. |
| `18-letteronly` | Displays all lines of `/etc/ssh/sshd_config` that **start with a letter** (A–Z or a–z). |
| `19-AZ` | Replaces all `A`→`Z` and `c`→`e` on input (using `tr`). |
| `20-hiago` | Removes all letters `c` and `C` from input. |
| `21-reverse` | Reverses its input (`rev`). |
| `22-users_and_homes` | Displays all users and their home directories from `/etc/passwd`, sorted by user (`user:home`). |
| `23-empty_casks` | Lists names of **empty** files and directories in CWD and subdirs (one per line, include hidden). No `basename`/`grep`. |
| `24-gifs` | Lists all `*.gif` files (recursively), **regular files only**, output names **without extension**, case-insensitive sort by byte value, one per line. No `basename`/`grep`. |
| `25-acrostic` | Decodes acrostics from STDIN using the **first letter** of each line; prints decoded message + newline. |
| `26-the_biggest_fan` | Parses TSV web logs from STDIN and prints the **top 11** hosts/IPs by request count (most first). No `grep`. |

## Notes
- You’re encouraged to **chain** tools (e.g., `cat … | grep … | cut … | sort … | uniq …`) to keep within the 2-line constraint.
- Be careful with quoting and escaping when dealing with special characters (especially in `7-file`).
- Read `man 5 passwd` and `man 5 shadow` to understand the fields you parse.

## Author
**Félix Besançon**  
Software Engineering Student @ Holberton School  
📧 f.besancon@hotmail.fr  
🔗 https://github.com/FelixBesancon
