# Computer Graphics by EDX

## Changes that were needed to get homeworks compiled on my ubuntu 18.04 machine:

* I needed to compile and copy different set of GL libraries from 
what has been distributed with the howmeworks. 
  ```
  hw0-linux_osx/lib/nix/**
  ```
* I needed to add the following to the `makefile` and the end of second `LDFLAGS` variables.
  ```
  -Wl,-rpath,./lib/nix
  ```