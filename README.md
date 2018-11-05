# bash

Ansible role to configure bash.
This sets up shared history between all bash instances.

## Variables
* `bash_max_history` (optional): Sets the maximum lines of history to keep, defaults to 1,000,000
* `bash_max_filesize` (optional): Sets the max file size of the bash history file, defaults to 1,000,000
* `bash_history_ignore_commands` (optional): List of commands to NOT include in the bash history, defaults to `ls` and `history`

## Optional Config
The following variables default to true. Set them to false to switch off the indicated functionality.
* `bash_collapse_multiline`: Collapses multiline commands into a single line in the bash history
* `bash_history_sharing`: Share the history between all active shells
* `bash_ignore_commands`: Configure bash history to ignore specific commands. The commands are defined by the `bash_history_ignore_commands` variable
* `bash_increased_history`: Configure increased bash history depth/retention period

