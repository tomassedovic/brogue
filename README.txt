**NOTE: This is NOT an official build of Brogue**

Go here for the official builds and code:

https://sites.google.com/site/broguegame/home

## Description ##

This fork adds support for `ctrl` and `shift` modifiers to the `left`
and `right` arrows, allowing diagonal movement with the arrow keys
(shift+arrow means "up", ctrl+arrow means "down") in the same way as
NotEye and e.g. ADOM do.

Personally, I like it much better than vi-keys on a laptop without a numpad.

Unfortunately, shift+arrow and ctrl+arrow combinations can't be set
with the custom keymap so we have to patch the code. To make matters
worse, those combinations are used for the "run in this direction"
functionality.

That means this functionality is unlikely to get merged upstream in
the current form, but I still like it enough to play this fork
instead.

## How to Build on Linux ##

You'll need to have your distro's equivalent of `SDL-devel` installed.

Run the following commands to produce a release tarball:

    $ make -f src/libtcod-1.5.2/Makefile release
    $ make tcod
    $ make tar


## Source Code and License

The basis for the fork comes from the official Brogue website:

https://sites.google.com/site/broguegame/home

specifically, the `brogue-1.7.5-linux-amd64.tbz2` file:

https://sites.google.com/site/broguegame/brogue-1.7.5-linux-amd64.tbz2?attredirects=0&d=1

Since the original Brogue is licensed under AGPL, so is this repo. See
the `agpl.txt` file for the full license text.

Tomas Sedovic <tomas@sedovic.cz>
