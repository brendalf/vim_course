# Integrating with Tmux
You can achieve even more productivity by integrating your workflow with tmux.
Tmux is a necessary tool in the tool belt of any software engineer, even if you
don't use vim.

## What is Tmux?
Tmux is an open source terminal multipleexer for Unix-like operating systems.
It allows multiple terminal sessions to be accessed simultaneously in a single
window.
It's useful for running more than one command-line program at the same time.

> You can also detach processes from their controlling terminals, allowing
> remote sessions to remain active without being visible.

## Tmux demo
Quick demo. For more information: https://tmuxcheatsheet.com/

### Manage session
**List sessions**:
`tmux ls`
`Ctrl+b s`

**Move between sessions**:
`Ctrl+b ) / Ctrl+b (`

**Rename a session**:
`Ctrl+b $`

**Detach from a session**:
`Ctrl+b d`

**New session**:
`tmux new -t SESSION_ID`

**Kill a session**:
`tmux kill-session -t SESSION_ID`

**Attach to a session**:
`tmux a -t SESSION_ID`

### Manage windows
**Create a window**:
`Ctrl+b c`

**Rename a window**:
`Ctrl+b ,`

**Move between windows**:
`Ctrl+b n / Ctrl+b p`
``Ctrl+b [0..9]``

### Panes
**Split pane horizontally**:
`Ctrl+b %`

**Split pane vertically**:
`Ctrl+b "`

**Show pane numbers**:
`Ctrl+b q`

**Close current pane**:
`Ctrl+b x`

**Toogle pane zoom**:
`Ctrl+b z`

**Move between panes**:
`Ctrl+b h / Ctrl+b j / Ctrl+b k / Ctrl+b l`

**Resize panes**:
`Ctrl+b+h / Ctrl+b+j / Ctrl+b+k / Ctrl+b+l`

### Copy Mode
**Enter copy mode**:
`Ctrl+b [`

**Start selection**:
`Spacebar`

**Clear selection**:
`Esc`

**Copy selection**:
`Enter`

**Paste selection**:
`Ctrl+b ]`

## Tmux configuration
You can configure your tmux using the file `.tmux.conf` in you home folder.
You can customize things like:
- Shortcuts
- Colour
- Basic Settings
- Powerline

