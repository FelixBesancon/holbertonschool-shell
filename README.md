# holbertonschool-shell

This repository contains my Shell scripting learning projects at Holberton School.  
It covers fundamental Unix command usage, shell scripting basics, file permissions, I/O redirections, and environment manipulation.

## Table of Contents
- [Description](#description)
- [Learning Objectives](#learning-objectives)
- [Requirements](#requirements)
- [Repository Structure](#repository-structure)
- [Projects](#projects)
  - [Project 0: Shell, basics](#project-0-shell-basics)
  - [Project 1: Shell, permissions](#project-1-shell-permissions)
  - [Project 2: Shell, I/O Redirections and filters](#project-2-shell-io-redirections-and-filters)
  - [Project 3: Shell, init files, variables and expansions](#project-3-shell-init-files-variables-and-expansions)
- [Author](#author)

## Description
This repository introduces Unix shell fundamentals and scripting through hands-on exercises.  
Each project covers a specific topic and contains executable scripts with strict constraints to encourage mastery of command-line logic and precision.

Each folder includes a dedicated `README.md` describing the behavior of every script.

## Learning Objectives
Across the projects in this repository:
- Understand what a shell is and how it works
- Navigate the filesystem and manipulate files/directories
- Use shell builtins and Unix command-line tools
- Manage file permissions and user groups
- Redirect input/output and use pipelines
- Filter data using commands such as `grep`, `sort`, `uniq`, `wc`, `tr`, etc.
- Work with shell variables, expansions, and shell arithmetic
- Configure shell initialization files and aliases

## Requirements
- OS: Ubuntu 20.04 LTS / Ubuntu 22.04 LTS
- Allowed editors: `vi`, `vim`, `emacs`
- All scripts are executable: `chmod +x filename`
- First line of every script: `#!/bin/bash`
- Each script must end with a new line
- No use of `&&`, `||`, `;` or backticks unless specified
- Adherence to project constraints specified by Holberton School

## Repository Structure
```
holbertonschool-shell/
├── README.md
├── basics/
│ └── README.md
├── permissions/
│ └── README.md
├── io_redirections_and_filters/
│ └── README.md
└── init_files_variables_and_expansions/
└── README.md
```

## Projects

### Project 0: Shell, basics
Introduction to shell commands and navigation:
- Filesystem navigation (`cd`, `pwd`, `ls`)
- Manipulating files and directories (`cp`, `mv`, `rm`, `mkdir`)
- Links, wildcards, and command help (`man`, `help`)
- Hidden files, permissions basics, long formats

See: `basics/README.md`

---

### Project 1: Shell, permissions
Understanding and manipulating Unix permissions:
- Users, groups and ownership
- Changing permissions with `chmod`
- Ownership modification (`chown`, `chgrp`)
- Symbolic / numeric modes
- Permissions on directories and symbolic links

See: `permissions/README.md`

---

### Project 2: Shell, I/O Redirections and filters
Input/output handling and text processing:
- Standard input/output redirection (`>`, `>>`, `<`)
- Pipelines (`|`)
- Filtering with `grep`, `uniq`, `wc`
- Sorting with `sort`
- File inspection and manipulation (`head`, `tail`, `cut`, `tr`)

See: `io_redirections_and_filters/README.md`

---

### Project 3: Shell, init files, variables and expansions
Shell configuration and scripting logic:
- Local and global variables
- Shell expansions (`$(( ))`, `${ }`)
- Command substitution (`$( )`)
- Aliases and initialization files (`.bashrc`, `.profile`)
- Arithmetic and base conversions
- Advanced text manipulation

See: `init_files_variables_and_expansions/README.md`

---

## Author
**Félix Besançon**  
Software Engineering Student @ Holberton School  
📧 f.besancon@hotmail.fr  
🔗 https://github.com/FelixBesancon
