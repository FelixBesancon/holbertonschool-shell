# Project 1: Shell, permissions

## Description
This project introduces Unix permissions and user/group management. You will practice changing file modes, owners and groups, working with symbolic links, viewing identity and groups, and using `sudo`/`su` appropriately. All scripts are minimal, executable, and follow strict formatting rules.

## Learning Objectives
By the end of this project, you should be able to explain:
- What file permissions are on Linux and how to read them
- How to represent owner/group/other permissions as a single digit
- How to change permissions (`chmod`), owner (`chown`) and group (`chgrp`)
- Why a normal user cannot `chown` files and how to use `sudo`/`su`
- How to run a command with root privileges
- How to print real/effective user and group IDs (`id`, `whoami`, `groups`)
- How to create users and groups

## Requirements
- Allowed editors: `vi`, `vim`, `emacs`
- Environment: Ubuntu 22.04 LTS
- **All scripts must be exactly two lines long** (`wc -l file` → `2`)
- All files must end with a new line
- The first line of every file must be exactly `#!/bin/bash`
- A `README.md` at the root of this project describing what each script does
- **Do not** use backticks, `&&`, `||`, or `;`
- All scripts must be executable (`chmod u+x <file>`)
- ⚠️ Tasks **3 / 13 / 14 / 15 / 16** must be run inside the sandbox for checker validation

## Files

| File | Description |
|------|-------------|
| `0-iam_betty` | Switches current user to `betty`. |
| `1-who_am_i` | Prints the effective username of the current user. |
| `2-groups` | Prints all groups the current user is part of. |
| `3-new_owner` | Changes the owner of file `hello` to `betty`. *(Must exist on GitHub and in `/tmp` on sandbox)* |
| `4-empty` | Creates an empty file named `hello`. |
| `5-execute` | Adds execute permission to the **owner** of `hello`. |
| `6-multiple_permissions` | Adds execute for owner and group; read for others, on `hello`. |
| `7-everybody` | Adds execute permission for owner, group and others on `hello` (no commas). |
| `8-James_Bond` | Sets `hello` perms to: owner **no perms**, group **no perms**, others **all perms** (no commas). |
| `9-John_Doe` | Sets the mode of `hello` to `-rwxr-x-wx` (no commas). |
| `10-mirror_permissions` | Sets the mode of `hello` the same as `olleh` (works for any mode). |
| `11-directories_permissions` | Adds execute to **all subdirectories** of CWD for owner, group, others (regular files unchanged). |
| `12-directory_permissions` | Creates directory `my_dir` with mode `751` in the working directory. |
| `13-change_group` | Changes the **group** owner of `hello` to `school`. *(Must exist on GitHub and `/tmp`)* |
| `14-change_owner_and_group` | Changes owner to `vincent` and group to `staff` for **all** files/dirs in CWD. *(Must exist on GitHub and `/tmp`)* |
| `15-symbolic_link_permissions` | Changes owner to `vincent` and group to `staff` of symbolic link `_hello` (not the target). *(Must exist on GitHub and `/tmp`)* |
| `16-if_only` | Changes owner of `hello` to `vincent` **only if** currently owned by `guillaume`. *(Must exist on GitHub and `/tmp`)* |

## Author
**Félix Besançon**  
Software Engineering Student @ Holberton School  
📧 f.besancon@hotmail.fr  
🔗 https://github.com/FelixBesancon
