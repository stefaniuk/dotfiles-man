# Bash

## Shortcuts

    ctrl+a ctrl+a   go to the beginning of the line
    ctrl+e          go to the end of the line
    ctrl+u          clear the line before the cursor position
    ctrl+k          clear the line after the cursor
    ctrl+z          put running job into a suspended background process, `fg` restores it
    ctrl+r          search through previously used commands

## Commands

    find . -type f -not -path "*/.git/*" -exec grep -Iq . {} \; -and -print0    # find text files only
        | xargs -0 dos2unix                                                     # convert line-endings
        | xargs -0 sed -E -i '' $'s/\t/    /g'                                  # replace tab by spaces
        | xargs -0 perl -pi -e 's/ +$//'                                        # trim whitespaces
    find . -type f -user 501 -exec chown 1000:staff {} \;                       # change ownership

    # Bootable USB stick from an ISO image
    diskutil list
    diskutil unmountDisk /dev/diskN
    sudo dd if=~/Downloads/image.iso of=/dev/rdiskN bs=1m
