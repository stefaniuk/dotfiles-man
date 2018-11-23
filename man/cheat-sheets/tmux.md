# Tmux

## Shortcuts

All of the following commands must be prefixed by the `ctrl+a` keyboard shortcut.

### Sessions

    s               list sessions
    :new<enter>     new session
    $               name session
    d               detach from session

### Windows

    c               create new window
    &               kill the current window
    n               next window
    p               previous window
    l               previously selected window
    <number>        specific window number
    w               list all windows
    .               move window
    ,               rename the current window

### Panes

    %               vertical split
    "               horizontal split
    x               kill pane
    o               go to the next pane (cycle through all of them)
    arrow           go to other pane in that direction
    ;               go to the previously selected pane
    q               show pane numbers
    q <number>      go to the specific pane number
    {               move the current pane left
    }               move the current pane right
    z               toggle pane zoom

### Misc

    :               prompt
    ?               list all key bindings
    ctrl+l ctrl+k   clear history (doesn't need the prefix)
    fn+up           scroll up, press q to quit
    fn+down         scroll down, press q to quit

## Commands

    tmux ls                         # list sessions
    tmux new -s <name>              # create new session
    tmux attach -t <name>           # attach to session
    tmux kill-session -t <name>     # kill session
    tmux lscm                       # list commands
    tmux source ~/.tmux.conf        # reload configuration
