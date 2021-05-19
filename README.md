# libffi tarballs for GHC

This repository contains the source tarballs used to
build [libffi](https://github.com/libffi/libffi/)
for [GHC](https://ghc.haskell.org/).

Note that in order to reduce working tree size, this repository contains only
orphan branches. Each branch contains one source tarball.

For some time these tarballs and their branches used to be generated using the
`mk-snapshot.sh` script because of the
[lack of releases](https://github.com/libffi/libffi/issues/296).
In order to update the `libffi` version built by GHC, first run
`mk-snapshot.sh`, then push the resulting branch to `git.haskell.org`, and
finally update the submodule commit in the `ghc` repository.
