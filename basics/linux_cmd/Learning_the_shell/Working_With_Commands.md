# Working With Commands
This lesson will introduce you the following commands.
- **type** - Display information about command type
- **which** - Locate a commands
- **help** - Display reference page for shell builtin
- **man** - Display an on-line commands reference

## What are "Commands"?
Commands can be one of 4 different kinds:
1. An executable program
2. A command built into the shell itself
3. A shell function
4. An alias

## Identifying Commands
### type
The **type** commands is a shell builtin that display the kind of commands the shell will execute, given a particular command name.
```bash
type command
```
```bash
[me@linuxbox me]$ type type
type is a shell builtin

[me@linuxbox me]$ type ls
ls is aliased to 'ls --color=tty'

[me@linuxbox me]$ type cp
cp is /bin/cp
```

### which
The **which** command is used to determine the exact location of a given executable.
```bash
[me@linuxbox me]$ which ls
/bin/ls
```

## Getting Command Documentation
### help
bash has a built-in help facility available for each of the shell builtins. To use it, type "help" followed by the name of shell builtin. Optionally, you may add the -m option to change the format of the output.

### --help
Many executable programs support a "--help" option that displays a description of the commands supported syntax and options.

### man
A special pagin program called **man** is used to view man page.
``` bash
[me@linuxbox me]$ man ls
```

### README And other documentation files
Many software packages installed on your system have documentation files residing in the /usr/share/doc directory.
use **less** or **zless** to view text and compressed text and use web-browser to view html 
<!--stackedit_data:
eyJoaXN0b3J5IjpbMjc3NTY2OTA4XX0=
-->