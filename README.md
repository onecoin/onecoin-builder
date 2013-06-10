onecoin-builder
===============

This is a set of bash scripts to cross-compile Onecoin Windows QT client on Linux.
These scripts can be easily adopted to build any Bitcoin-QT derivative.

Usage
-----

1.  Edit `vars` if needed.
2.  Run `./download` to fetch dependencies' tarballs (or put them into `deps/`
    dir).
3.  Run `./build-deps` to compile all of dependencies, or any of other `./build-*`
    scripts to build them one by one.
4.  Place Onecoin sources into `onecoin/` directory.
    `git clone https://github.com/onecoin/onecoin.git onecoin` is probably the
    easiest way.
5.  Run `./build-project` to compile the Windows binary. It may be found in
    `onecoin/release/` dir then.

Notes
-----

QT is compiled as statical library, and the resulting executable is statically
linked, so there is no DLLs needed to run it.

Credits
-------

This project is inspired by VirtualDestructor's
[build scripts](https://github.com/VirtualDestructor/bitcoin-qt-i2p).
