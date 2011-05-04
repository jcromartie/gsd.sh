# gsd.sh: Get S#!t Done

`gsd.sh` is a simple shell script to improved productivity by blocking
sites through modifying `/etc/hosts`, creating an entry pointing to
127.0.0.1 for each site in a list.

## Installation

Copy `gsd.sh` to somewhere in your `PATH`. For convenience, you may
wish to create an alias like this:

    alias gsd="sudo -E gsd.sh"

If you're not on Mac OS X, also set `GSD_RESET` to the command used to
reload `/etc/hosts`.

## Usage

Simply run the script to set your hosts file to "work mode."

    sudo -E gsd.sh

To go back to "play mode" run:

    sudo -E gsd.sh --play

## Customizing

Just Set the environment variable `GSD_SITES` to **add** to the
default list of sites.
