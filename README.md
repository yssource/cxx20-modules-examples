# C++20 Modules Examples

This repository contains a number of examples that demonstrate various C++20
modules features and their support in `build2`.

[`hello-module`][hello-module]                     -- module example

[`hello-partition`][hello-partition]               -- module partition example

[`hello-header-import`][hello-header-import]       -- header unit importation example

[`hello-header-translate`][hello-header-translate] -- header include translation example

[`hello-library-module`][hello-library-module]     -- module library example

[`hello-library-header`][hello-library-header]     -- header importation/translation library example

[hello-module]:           https://github.com/build2/cxx20-modules-examples/tree/master/hello-module
[hello-partition]:        https://github.com/build2/cxx20-modules-examples/tree/master/hello-partition
[hello-header-import]:    https://github.com/build2/cxx20-modules-examples/tree/master/hello-header-import
[hello-header-translate]: https://github.com/build2/cxx20-modules-examples/tree/master/hello-header-translate
[hello-library-module]:   https://github.com/build2/cxx20-modules-examples/tree/master/hello-library-module
[hello-library-header]:   https://github.com/build2/cxx20-modules-examples/tree/master/hello-library-header

While you can build each example individually (see `README` in each example
for details), you can also build them all at once in a shared build
configuration, for example:

```
git clone https://github.com/build2/cxx20-modules-examples.git
cd cxx20-modules-examples

bdep init -C @gcc cc config.cxx=g++ config.cxx.translate_include=all-importable
bdep update @gcc
```
