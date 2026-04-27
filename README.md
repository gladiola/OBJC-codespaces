# OBJC-codespaces

Sample repo to set up codespaces for use with Objective-C and GNUstep on OpenBSD.

## Prerequisites

Install GNUstep on OpenBSD using the package manager:

```sh
pkg_add gnustep-make gnustep-base libobjc2
```

After installation, source the GNUstep environment script to configure your shell:

```sh
. /usr/local/share/GNUstep/Makefiles/GNUstep.sh
```

You may add this line to your `~/.profile` so it is applied automatically on login.

## Building

With the GNUstep environment sourced, run `make` from the repository root:

```sh
make
```

This compiles `HelloWorld.m` using the GNUstep build system and produces the
`HelloWorld` executable inside the `obj/` directory created by GNUstep make.

## Running

```sh
./obj/HelloWorld
```

Expected output:

```
Hello, World!
```

## Cleaning

```sh
make clean
```
