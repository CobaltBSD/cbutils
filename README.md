# cbtutils (Cobalt Utils)

An assortment of various UNIX system utilities ported to Cobalt from a wide variety of sources. Most of these are ported from various UNIX-like sources that are not GNU/Linux. A few of these, such as our version of `ls`, are heavily modified from their original ported form to support additional functionality.

## Utils
* banner - Displays an ASCII art text banner (Ported from Heirloom)
* bs - Battleship game (Ported from OpenBSD)
* fortune - Displays a random message from a database (Ported from OpenBSD)
* freq - Displays a histogram of character frequencies (Ported from Plan9)
* grdc - Terminal digital clock (Ported from OpenBSD)
* locale - Displays locale environment variables (Ported from OpenBSD)
* ls - List files (Forked from OpenBSD; heavily modified)
* news - Displays news items as they appear in a directory (Ported from Plan9)
* number - Displays a text-representation of a number in digits (Ported from OpenBSD)
* primes - Display primes in a selected range of numbers (Ported from OpenBSD)
* rs - Columnate a list of entries (Ported from NetBSD)
* tetris - Tetris game (Ported from OpenBSD)
* unicode - Display unicode characters corresponding to a number (Ported from Plan9)
* units - Convert between different units (Ported from OpenBSD)
* unutf - Convert characters into their corresponding number (Ported from Plan9)
* getent - Get database entries (Ported from Alpine Linux, which was in turn ported from NetBSD)
* c89 - POSIX c89 compatibility program (Ported from FreeBSD)
* c99 - POSIX c99 compitibility program (Ported from FreeBSD)
* entropy - Prints the entropy of stdin using zxcvbn (Requires [zxcvbn-c](https://github.com/tsyrogit/zxcvbn-c); see below for installation tips)

cbtutils requires [crunchgen-ng](https://github.com/CobaltBSD/crunchgen-ng) to build.

## ZXCVBN-C installation
cbtutils includes a command-line tool for calculating passphrase entropy using zxcvbn. If you wish to avoid this requirement, you can remove the referenced to `zxcvbn` and `entropy` from cbtutils.conf. Otherwise, you will also need to install one of the `.dict` dictionaries from the zxcvbn-c source directory to `/usr/share/misc/zxcvbn.dict`.

## License
cbtutils is available under a wide variety of licenses, as the components of it come from a large number of sources. For all other components of cbtutils (e.g. the makefiles), 0BSD license applies. See `LICENSE`
