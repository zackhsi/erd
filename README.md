ERD tooling
===========

Based on: https://github.com/BurntSushi/erd.

Watch an ER file, outputting a PDF to ~/Desktop on updates.

Installation
------------

```sh
# Install graphviz.
$ brew install graphviz --with-pango
# Install Haskell toolchain.
$ brew install ghc cabal-install
# Install erd.
$ cabal install --allow-newer erd 
# Symlink erd into $PATH.
$ ln -s ~/.cabal/bin/erd /usr/local/bin/
# Install fswatch to automatically rebuild.
$ brew install fswatch
```

Usage
-----

```sh
# Run watch process in background.
$ ./erd-watcher <file-to-watch>
```
