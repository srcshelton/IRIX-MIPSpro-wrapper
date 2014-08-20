IRIX-MIPSpro-wrapper
====================

A tool to mangle compiler and binutils arguments to automagically insert the library paths and includes required to build software successfully in a prefix-portage environment.

More generally, the IRIX-MIPSpro-wrapper script will perform a translation of GNU `gcc` front-end compiler arguments to provide input suitable for passing to MIPSpro tools.  Where well-known common packages require specific work-arounds, these are also implemented, as are all MIPSpro options which have a direct or indirect mapping to `gcc` arguments.

This should allow for the MIPSpro suite to be used in place of `gcc` in most cases, without any need for specific MIPSpro support on the part of the source code being compiled.

Required tools:

* SGI MIPSpro 7.4.4m compiler suite (untested on earlier releases);

* GNU `bash` 3 or higher;

* `/bin/uname`, `/sbin/hinv`;

* `readlink`, `touch`, `tr`, `grep`, `cut`, GNU `sed`, `sort`, `head`, `basename`.

Version `20100316.1`.
