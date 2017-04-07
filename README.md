# Linking with `lld` in Haskell builds

**10x faster** than `ld` in the linkin steps, **3x faster** than `gold`.

Use `cabal configure --with-gcc=clang --with-ld=clang`, then `cabal build`.

See the `.cabal` file for what options are needed.

## Bugs

cabal bugs that prevent using `lld` in the library linking step:

* [cabal does not respect ghc-options for -pgmc, -pgml etc](https://github.com/haskell/cabal/issues/4439)
