This is a C library which can be used in deep learning applications.  It allows multiple layers to be trained and also includes the dropouts technique to avoid overfitting the data.

Installation
============

To build from source:

```bash
make
sudo make install
```

This creates the library and installs it into /usr/local

Unit Tests
==========

You can run the unit tests to check that the system is working as expected:

```bash
make tests
./tests
```

Or to check for any memory leaks:

```bash
valgrind --leak-check=full ./tests
```

Examples
========

There are also some example programs within the examples directory. Reading the examples is the best way to learn how to use this library within your own code.

Portability
===========

Although this software was primarily written to run on Linux-based systems it's pretty much just vanilla C code and so it should be easily portable to other platforms, such as Microsoft Windows and Mac systems. The independent random number generator should mean that results are consistent across different compilers and platforms.

Packaging
=========

To build packages for Debian (deb) or Fedora (rpm) based systems there are two scripts, debian.sh and fedora.sh which can be used to generate packages for convenient installation.
