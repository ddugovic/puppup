# Puppup: Basic crossword game engine

Suggests moves for OMGWords crossword games using a [gaddag](https://en.wikipedia.org/wiki/GADDAG).

![screenshot](https://pics.dllu.net/file/dllu-sc/1485531d49.png)

# About

A GADDAG is a type of directed acyclic word graph (DAWG) where each word is stored with each of its prefixes, reversed.

![puppup](https://daniel.lawrence.lu/puppy/puppup.png)

**Figure 1**: A small purple dawg and its reverse.

# Build

You need CMake and a reasonably new GCC or Clang compiler supporting C++14.

```
cmake . -DCMAKE_BUILD_TYPE=Release
make
```

# Running

Puppup outputs [ANSI colour codes](https://en.wikipedia.org/wiki/ANSI_escape_code#Colors), so be sure to use a terminal that supports this.
You need to supply your own dictionary (a text file with one word per line).

```
./puppup CEL/cel.txt
```
