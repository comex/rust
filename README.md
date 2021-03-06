# The Rust Programming Language

This is a compiler for Rust, including standard libraries, tools and
documentation.

## Quick Start

### Windows

1. Download and use the [installer and MinGW][win-wiki].
2. Read the [tutorial].
2. Enjoy!

> ***Note:*** Windows users can read the detailed
> [getting started][wiki-start] notes on the wiki.

[tutorial]: http://static.rust-lang.org/doc/tutorial.html
[wiki-start]: https://github.com/mozilla/rust/wiki/Note-getting-started-developing-Rust
[win-wiki]: https://github.com/mozilla/rust/wiki/Using-Rust-on-Windows

### Linux / OS X

1. Make sure you have installed the dependencies:
    * `g++` 4.4 or `clang++` 3.x
    * `python` 2.6 or later (but not 3.x)
    * `perl` 5.0 or later
    * GNU `make` 3.81 or later
    * `curl`
2. Download and build Rust:

    You can either download a [tarball] or build directly from the [repo].

    To build from the [tarball] do:

        $ curl -O http://static.rust-lang.org/dist/rust-0.9.tar.gz
        $ tar -xzf rust-0.9.tar.gz
        $ cd rust-0.9

    Or to build from the [repo] do:

        $ git clone https://github.com/mozilla/rust.git
        $ cd rust

    Now that you have Rust's source code, you can configure and build it:

        $ ./configure
        $ make && make install

    > ***Note:*** You may need to use `sudo make install` if you do not normally have
    > permission to modify the destination directory. The install locations can
    > be adjusted by passing a `--prefix` argument to `configure`. Various other
    > options are also supported, pass `--help` for more information on them.

    When complete, `make install` will place several programs into
    `/usr/local/bin`: `rustc`, the Rust compiler; `rustdoc`, the
    API-documentation tool, and `rustpkg`, the Rust package manager and build
    system.
3. Read the [tutorial].
4. Enjoy!

[repo]: https://github.com/mozilla/rust
[tarball]: http://static.rust-lang.org/dist/rust-0.9.tar.gz
[tutorial]: http://static.rust-lang.org/doc/0.9/tutorial.html

## Notes

Since the Rust compiler is written in Rust, it must be built by a
precompiled "snapshot" version of itself (made in an earlier state of
development). As such, source builds require a connection to the Internet, to
fetch snapshots, and an OS that can execute the available snapshot binaries.

Snapshot binaries are currently built and tested on several platforms:

* Windows (7, Server 2008 R2), x86 only
* Linux (various distributions), x86 and x86-64
* OSX 10.6 ("Snow Leopard") or greater, x86 and x86-64

You may find that other platforms work, but these are our officially
supported build environments that are most likely to work.

Rust currently needs about 1.5 GiB of RAM to build without swapping; if it hits
swap, it will take a very long time to build.

There is a lot more documentation in the [wiki].

[wiki]: https://github.com/mozilla/rust/wiki

## License

Rust is primarily distributed under the terms of both the MIT license
and the Apache License (Version 2.0), with portions covered by various
BSD-like licenses.

See LICENSE-APACHE, LICENSE-MIT, and COPYRIGHT for details.
