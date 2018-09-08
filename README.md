# CLI-Chess-Rating-Getter
A UNIX/Linux/Mac command-line tool to get a player's current rating from the US Chess Website.

This program was written and tested on a Mac.

Dependencies:
 - bash
 - curl
 - An internet connection

Installation:
Just download or copy/paste into a text file, then run `chmod u+x <filename>`.

How to Use:
 - From `getrating --help`:

    Usage: getrating [ --quick | -q | --blitz | -b ] --default-id | -d | <US CHESS ID>
        This program gets a player's chess rating from the US Chess website."
        By default, a player's regular rating is retrieved."
        If --quick or --blitz is specified, the player's quick or blitz rating is retrieved."
        The --default-id option tells the program to use the default US Chess ID, which is"
          stored in the $MY_USCF_ID environment variable.'
