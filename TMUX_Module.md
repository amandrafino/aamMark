
# TMUX Module

## Introduction to TMUX
TMUX is a terminal multiplexer that allows users to access multiple separate terminal sessions inside a single terminal window or remote terminal session. It is useful for running more than one command-line program at the same time.

## Getting Started with TMUX
### Installation
- On Ubuntu/Debian: `sudo apt-get install tmux`
- On CentOS/RHEL: `sudo yum install tmux`
- On macOS: `brew install tmux`

### Starting a New Session
- To start a new TMUX session, simply type `tmux` in your terminal.
- You can also start a new session with a custom name using `tmux new -s my_session`.

### Basic Commands
- `Ctrl + b` is the default prefix key in TMUX. Most TMUX commands start with this prefix.
- To create a new window, press `Ctrl + b` then `c`.
- To switch between windows, press `Ctrl + b` then a window number (e.g., `0`, `1`, `2`, etc.).
- To switch between windows, press 'Ctrl + b' then `p` or `n'
- To split the current window vertically, press `Ctrl + b` then `%`.
- To split the current window horizontally, press `Ctrl + b` then `"`.
- To close the current pane or window, type `exit` or press `Ctrl + d`.

### Detaching and Attaching Sessions
- To detach from a session and return to your normal terminal, press `Ctrl + b` then `d`.
- To list all sessions, type `tmux ls` in the terminal.
- To re-attach to a specific session, use `tmux attach-session -t my_session`.

### Rename Windows and Remove Windows
- To rename a window press `Ctrl + b` then `,`
- To remove a window press `Ctrl + b' then `&`

## Tips for Beginners
- Customize your TMUX configuration by creating and editing `~/.tmux.conf`.
- Learn keyboard shortcuts to navigate efficiently.
- Use TMUX sessions to manage multiple tasks and projects.
- Explore plugins and additional features to enhance your TMUX experience.


## Conclusion
TMUX is a powerful tool for managing terminal sessions, especially for users who work extensively in the command line. With practice, it becomes an invaluable part of your workflow.

---
Generated for Albert as part of a programming and prompt engineering mentorship program.
