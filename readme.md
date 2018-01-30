![Hackage](https://img.shields.io/hackage/v/iwlib.svg)

# About

*iwlib* is a thin wrapper over the *iw* C library, providing access to
wireless card information in supported systems.

# Bug Reports

To submit bug reports you can use the [bug tracker over at Github].

[bug tracker over at Github]: https://github.com/jaor/iwlib/issues

# Installation

## Using cabal-install

iwlib is available from [Hackage], and you can install it using
`cabal-install`:

        cabal install iwlib

## From source

If you don't have `cabal-install` installed, you can get iwlib's
source code in a variety of ways:

  - From [Hackage]. Just download the latest release from xmobar's
    hackage page.
  - From [Github]. You can also obtain a tarball in [Github's
    downloads page]. You'll find there links to each tagged release.
  - From the bleeding edge repo. If you prefer to live dangerously,
    just get the latest and greatest (and buggiest, I guess) using
    git:

        git clone git://github.com/jaor/iwlib


[Github's downloads page]: https://github.com/jaor/iwlib/downloads

If you have cabal installed, you can now use it from within its source
tree:

        cabal install


Otherwise, run the configure script:

        runhaskell Setup.lhs configure

Now you can build the source:

        runhaskell Setup.lhs build
        runhaskell Setup.lhs install # possibly to be run as root

# External dependencies

No other Haskell library is required, but you will need the [iwlib] C
library and headers in your system (e.g., install `libiw-dev` in
Debian-based systems or `wireless_tools` on Arch Linux).

# Authors

This library is written and maintaned by Jose Antonio Ortega Ruiz.

# Thanks

Many thanks to Leif Warner for suggesting the creation of this library
and providing the initial hackage scaffolding.

# License

This software is released under a BSD-style license. See [LICENSE] for
more details.

Copyright &copy; 2018 Jose Antonio Ortega Ruiz

[Github]: http://github.com/jaor/iwlib/
[Github page]: http://github.com/jaor/iwlib
[Hackage]: http://hackage.haskell.org/package/iwlib/
[LICENSE]: https://github.com/jaor/iwlib/raw/master/license
[iwlib]: http://www.hpl.hp.com/personal/Jean_Tourrilhes/Linux/Tools.html
