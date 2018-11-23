Dotfiles Extension: Manuals
===========================

My notes on how to use and configure various command-line tools as a set of text files.

Installation
------------

Install this extension using the [`dotfiles`](https://github.com/stefaniuk/dotfiles) command.

    $ ~/dotfiles --extension-man
    $ reload

Usage
-----

    $ dman --help

    Usage: dotfiles-man term1 [term2 term3 ...]

    Options:
            -a|--list-all
            -r|--show-raw
            -h|--help

    $ dman -r versioning    # Show it in the terminal
    $ dman versioning       # Show it in a browser

Development
-----------

    $ alias dman="./usr/bin/dotfiles-man"
