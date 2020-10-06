# CLI-Chess-Rating-Getter
A UNIX command-line tool to get a player's current rating from the US Chess website.

### Important dependencies:
 - `curl`
 - An internet connection

### How to Use:
From `getrating --help`:
```
Usage: getrating [ --quick | -q | --blitz | -b ] --default-id | -d | <US CHESS ID>
    This program gets a player's chess rating from the US Chess website.
    By default, a player's regular rating is retrieved.
    If --quick or --blitz is specified, the player's quick or blitz rating is retrieved.
    The --default-id option tells the program to use the default US Chess ID, which is
     stored in the $MY_USCF_ID environment variable.
```

### How it works
This script uses a semi-hidden mininal rating lookup page on uschess.org (use it like this: http://www.uschess.org/msa/thin3.php?12345678). See "'Thin' client access to MSA data" in http://www.uschess.org/msa/Index.php .

This program was written and tested on a Mac, but it should work on Unix-ish systems.

### Interested in contributing?
This program needs to be reworked to use GNU `getopt`.
