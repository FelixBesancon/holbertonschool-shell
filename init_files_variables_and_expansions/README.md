# Project 3: Shell — Init Files, Variables and Expansions

## Description
This project explores **shell initialization files**, **environment/local variables**, **expansions** (parameter/command/arithmetic), **quoting**, **aliases**, and a handful of utilities for printing and formatting. Scripts are intentionally minimal and follow strict formatting rules.

## Learning Objectives
By the end, you should be able to explain:
- What happens when running `ls -l *.txt` (globbing → command execution).
- The role of `/etc/profile`, `/etc/profile.d/`, and `~/.bashrc`.
- Differences between **local** vs **environment** variables; how to create, update, delete.
- Reserved variables like `HOME`, `PATH`, `PS1`; special parameters (`$?`, `$#`, `"$@"`, etc.).
- Expansions: parameter, command substitution `$( )` / backticks, arithmetic `$(( ))`.
- Quoting rules (single vs double quotes).
- Basic shell arithmetic.
- `alias` / `unalias` and how to temporarily bypass aliases.
- Executing commands from a file in the **current shell** (`.` / `source`).

## Requirements
- Allowed editors: `vi`, `vim`, `emacs`
- Environment: Ubuntu **20.04 LTS**
- **All scripts must be exactly two lines** (`wc -l file` → `2`)
- All files must end with a newline
- First line of each file: `#!/bin/bash`
- A `README.md` in this folder describing each script
- **Do not** use `&&`, `||`, or `;`
- **Do not** use `bc`, `sed`, or `awk`
- All scripts must be executable (`chmod u+x <file>`)

## Files

| File | Description |
|------|-------------|
| `0-alias` | Creates an alias `ls='rm -f *'`. |
| `1-hello_you` | Prints `hello <user>` where `<user>` is the current login (`$USER`). |
| `2-path` | Appends `/action` to the end of `PATH`. |
| `3-paths` | Prints the **number of directories** in `PATH` (handles empty entries). |
| `4-global_variables` | Lists **environment variables** (`printenv`-style output). |
| `5-local_variables` | Lists **all** shell variables, environment variables, and functions. |
| `6-create_local_variable` | Creates a **local** variable `BEST=School`. |
| `7-create_global_variable` | Creates an **environment** variable `BEST=School` (`export`). |
| `8-true_knowledge` | Prints `128 + $TRUEKNOWLEDGE`. |
| `9-divide_and_rule` | Prints `$POWER / $DIVIDE`. |
| `10-love_exponent_breath` | Prints `$BREATH` to the power of `$LOVE`. |
| `11-binary_to_decimal` | Converts binary in `$BINARY` to **base 10**. |
| `12-combinations` | Prints all 2-letter lowercase combinations (aa…zz) except `oo`, alpha-sorted; one per line; ≤ 64 chars in the script file. |
| `13-print_float` | Prints `$NUM` with **two decimal places**. |
| `14-decimal_to_hexadecimal` | Converts decimal in `$DECIMAL` to **hex** (lowercase). |
| *(blog)* | **What happens when you type `ls *.c`** — published post (see link below). |
| `15-rot13` | (Advanced) Encodes/decodes input with **rot13** (ASCII). |
| `16-odd` | (Advanced) Prints **every other line** from STDIN, starting with the first. |
| `17-water_and_stir` | (Advanced) Adds numbers from `$WATER` (base *water*) and `$STIR` (base *stir*); prints result in base *bestchol*. |

## Notes
- Many tasks require **parameter expansion** + **arithmetic expansion** and/or **command substitution** in a single concise pipeline to stay within the 2-line constraint.
- To bypass an alias temporarily, prefix with a backslash (e.g., `\ls`).
- Read `man` pages: `printenv`, `set`, `unset`, `export`, `alias`, `unalias`, `.`, `source`, `printf`.

## Blog Post (Advanced Task)
- **“What happens when you type `ls *.c`”**  
  https://medium.com/@f.besancon/what-happens-when-you-type-ls-c-ec691e743936

## Author
**Félix Besançon**  
Software Engineering Student @ Holberton School  
📧 f.besancon@hotmail.fr  
🔗 https://github.com/FelixBesancon
