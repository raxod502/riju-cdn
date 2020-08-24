# Riju CDN

This repository contains assets hosted for
[Riju](https://github.com/raxod502/riju). Why?

* Haskell package management is one of the worst atrocities ever to
  blight this earth, hence installing any Haskell packages in the
  build system of Riju is basically impossible. I compile them
  manually, do some *real jank sh\*\** to fix hardcoded dependencies
  on arbitrary features of the build environment, and then upload them
  here so they can be downloaded by Riju.
* Some people just don't know how to run CDNs. Ironically enough Apple
  is one such company; the official download for Swift fails on a
  regular basis. I mirror the files here, because MicrosoftHub knows
  what they're doing when it comes to file hosting. Sourceforge has
  similar problems.

## Maintenance

Unfortunately, I did not keep a record of how I prepared all of these
files. Next time I need to update one of them, I'll figure it out and
write it down.

### Brittany

Install latest version of Cabal v3, then use it with `--installdir` to
create a binary linked to `/usr/lib/ghc`.

### Ezhil

Download latest tarball from
[Sourceforge](https://sourceforge.net/projects/ezhillang/files/Linux-Ubuntu-64bit/).

### Unison

Follow the instructions at [the
README](https://github.com/unisonweb/unison#building-using-stack),
namely just `stack build` and then extract the binary from `stack exec
which unison`.
