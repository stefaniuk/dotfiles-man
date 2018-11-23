# Bash

## Shortcuts

    ctrl+a ctrl+a   go to the beginning of the line
    ctrl+e          go to the end of the line
    ctrl+u          clear the line before the cursor position
    ctrl+k          clear the line after the cursor
    ctrl+z          put running job into a suspended background process, `fg` restores it
    ctrl+r          search through previously used commands

## Commands

    find . -type f -exec dos2unix {} \;                     # convert line-endings
    find . -type f -print0 | xargs -0 perl -pi -e 's/ +$//' # trim whitespace
    find . -type f -user 501 -exec chown 1000:staff {} \;   # change ownership
