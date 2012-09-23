gyp-skeleton
=======

*gyp-skeleton* is intended to be a skeleton project to get up and running with
the [gyp](http://code.google.com/p/gyp/) build configuration system. gyp can be
used in the same capacity as [GNU
autotools](http://en.wikipedia.org/wiki/GNU_build_system) or
[CMake](http://www.cmake.org/), but is intended to be much simpler.

gyp separates the decision engine of a build from the execution engine -- gyp
has several backends, the most common being Visual Studio and traditional
Makefiles. This project focuses on Makefiles, but could be extended to generate
VS projects as well.

building
========

```
    sudo aptitude install build-essential gyp
    build/gen_makefile.sh
    make
```

and the output will be in `out/Default/hello`. There is an additional script
`build/clean_all.sh` which will remove all buildsystem-generated files and
outputs.
