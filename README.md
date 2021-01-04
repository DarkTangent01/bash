Shortcuts of Bash
=====================

> Mayank Srivastava

## Moving

| command  | description                    |
|----------|--------------------------------|
| ctrl + a | Goto BEGINNING of command line |
| ctrl + e | Goto END of command line       |
| ctrl + b | move back one character        |
| ctrl + f | move forward one character     |
| alt + f  | move cursor FORWARD one word   |
| alt + b  | move cursor BACK one word      |
| ctrl + ] + x	 | Where x is any character, moves the cursor forward to the next occurance of x |
| alt + ctrl + ] + x  | Where x is any character, moves the cursor backwards to the previous occurance of x |

## Other

| command  | description                    |
|----------|--------------------------------|
| ctrl + d          | Delete the character under the cursor |
| ctrl + h          | Delete the previous character before cursor |
| ctrl + u          | Clear all BEFORE cursor |
| ctrl + k          | Clear all AFTER cursor |
| ctrl + w          | delete the word BEFORE the cursor |
| alt + d           | delete the word FROM the cursor |
| ctrl + l          | Clear the screen (same as clear command) |
| ctrl + c          | kill whatever is running |
| ctrl + d          | Exit shell (same as exit command) |
| ctrl + t          | swap the last two characters before the cursor |
| ctrl + y          | paste (if you used a previous command to delete) |
| ctrl + z          | Place current process in background |
| ctrl + _          | undo |
| ctrl + x ctrl + u	| Undo the last changes. ctrl+ _ does the same |
| esc + t           | Swap last two words before the cursor |
| esc + .           | |
| esc + _           | |
| alt + [Backspace] | delete PREVIOUS word |
| alt + <           | Move to the first line in the history |
| alt + >           | Move to the end of the input history, i.e., the line currently being entered |
| alt + ?           | |
| alt + *           | |
| alt + .           | print the LAST ARGUMENT (ie "vim file1.txt file2.txt" will yield "file2.txt") |
| alt + c           | |
| alt + l           | |
| alt + n           | |
| alt + p           | Non-incremental reverse search of history. |
| alt + r           |Undo all changes to the line|
| alt + ctl + e     |Expand command line. |
| alt + t           | |
| alt + u           | |
| ~[TAB][TAB]       | List all users |
| $[TAB][TAB]       | List all system variables |
| @[TAB][TAB]       | List all entries in your /etc/hosts file |
| [TAB]             | Auto complete |
| cd -              | change to PREVIOUS working directory |

## History

| command  | description                    |
|----------|--------------------------------|
| ctrl + r          | Search backward starting at the current line and moving 'up' through the history as necessary |
| crtl + s          | Search forward starting at the current line and moving 'down' through the history as necessary |
| ctrl + p          | Fetch the previous command from the history list, moving back in the list (same as up arrow) |
| ctrl + n          | Fetch the next command from the history list, moving forward in the list (same as down arrow) |
| ctrl + o          | Execute the command found via Ctrl+r or Ctrl+s |
| ctrl + g          | Escape from history searching mode |
| !!                | Run PREVIOUS command (ie `sudo !!`) |
| !vi               | Run PREVIOUS command that BEGINS with vi |
| !vi:p             | Print previously run command that BEGINS with vi |
| !n		            | Execute nth command in history |
| !$		            | Last argument of last command |
| !^		            | First argument of last command |
| ^abc^xyz	        | Replace first occurance of abc with xyz in last command and execute it |

# Kill a job

n = job number, to list jobs, run `jobs`

```bash
kill %n
```

Example:

```bash
kill %1
```
