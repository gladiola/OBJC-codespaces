# OBJC-codespaces

Sample repo to set up codespaces for use with Objective-C and GNUstep on OpenBSD.

## Prerequisites

Install GNUstep on OpenBSD using the package manager:

```sh
pkg_add gnustep-make gnustep-base libobjc2
```

## Building

Run `make` from the repository root:

```sh
make
```

This compiles `HelloWorld.m` using `cc` with the GNUstep and libobjc2 flags and
produces the `HelloWorld` executable in the repository root.

## Running

```sh
./HelloWorld
```

Expected output:

```
Hello, World!
```

## Cleaning

```sh
make clean
```
