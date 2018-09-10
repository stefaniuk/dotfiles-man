    diskutil list
    diskutil unmount /dev/(IDENTIFIER)
    sudo dd if=image.iso of=/dev/r(IDENTIFIER) bs=1m
