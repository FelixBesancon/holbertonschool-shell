# Project 0: Shell, basics

## Description
This project introduces the Unix shell and core filesystem/navigation commands. You will practice reading man pages, using built-ins and external commands, handling options/arguments, listing files (including hidden ones), creating/moving/deleting files and directories, and working with links and wildcards. All scripts are minimal, executable, and follow strict formatting rules.

## Learning Objectives
By the end of this project, you should be able to explain:
- What the shell is, what a terminal is, and what the shell prompt represents
- What a shebang is and why we use `#!/bin/bash`
- The basics of command history and how to read man pages
- Navigation: `pwd`, `cd`, `ls`, `.` and `..`, home vs. root directories, hidden files
- Looking around: `ls`, `less`, `file`, long listing format
- Links: hard vs. symbolic (`ln`)
- File operations: `cp`, `mv`, `rm`, `mkdir`
- Command discovery: `type`, `which`, `help`, `man`, and when to use each
- Wildcards (globbing) and how to apply them
- What LTS means

## Requirements
- Allowed editors: `vi`, `vim`, `emacs`
- Environment: Ubuntu 22.04 LTS
- **All scripts must be exactly two lines long** (`wc -l file` → `2`)
- All files must end with a new line
- The first line of every file must be exactly `#!/bin/bash`
- A `README.md` at the root of the repository describing the repository
- A `README.md` at the root of this project describing what each script does
- **Do not** use backticks, `&&`, `||`, or `;`
- All scripts must be executable (`chmod u+x <file>`)

## Files

| File | Description |
|------|-------------|
| `0-current_working_directory` | Prints the absolute path of the current working directory (`pwd`). |
| `1-listit` | Displays the contents of the current directory (`ls`). |
| `2-bring_me_home` | Changes the working directory to the user’s home directory. |
| `3-listfiles` | Displays current directory contents in long format (`ls -l`). |
| `4-listmorefiles` | Displays current directory contents including hidden files, long format (`ls -la`). |
| `5-listfilesdigitonly` | Long format, numeric user/group IDs, including hidden files (`ls -la -n`). |
| `6-firstdirectory` | Creates directory `/tmp/my_first_directory`. |
| `7-movethatfile` | Moves file `betty` to `/tmp/my_first_directory/`. |
| `8-firstdelete` | Deletes the file `betty` in `/tmp/my_first_directory/`. |
| `9-firstdirdeletion` | Deletes directory `/tmp/my_first_directory`. |
| `10-back` | Changes the working directory to the previous one. |
| `11-lists` | Lists files in current dir, parent of working dir, and `/boot` (in this order), long format, including hidden files. |
| `12-file_type` | Prints the type of the file named `iamafile` in `/tmp` (`file /tmp/iamafile`). |
| `13-symbolic_link` | Creates a symbolic link named `__ls__` to `/bin/ls` in the current directory. |
| `14-copy_html` | Copies all `.html` files to the parent directory **only if** they don’t exist there or are newer. |
| `15-lets_move` | Moves all files beginning with an uppercase letter to `/tmp/u`. |
| `16-clean_emacs` | Deletes all files in current directory ending with `~`. |
| `17-tree` | Creates the directories `welcome/`, `welcome/to/`, and `welcome/to/school/` in the current directory (two spaces/lines only). |

## Author
**Félix Besançon**  
Software Engineering Student @ Holberton School  
📧 f.besancon@hotmail.fr  
🔗 https://github.com/FelixBesancon
