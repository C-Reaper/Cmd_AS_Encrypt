# Project README

## Overview
This project is a C/C++ application that demonstrates RSA encryption using the GMP library for large number arithmetic. It includes functionality to generate large prime numbers, compute modular exponentiation, and perform RSA encryption/decryption.

## Features
- RSA 2048-bit key generation
- Modular exponentiation for encryption and decryption
- Conversion between strings and large integers using GMP
- Large random prime number generation

## Project Structure
### Prerequisites
- C/C++ Compiler (GCC, Clang)
- Make utility
- Standard development tools
- Libraries:
  - GMP library for arbitrary precision arithmetic
  - OpenSSL for secure randomness

## Build & Run
The project includes four Makefiles for different operating systems:

### Linux
To build and run the application on a Linux system:
```sh
cd <Project>
make -f Makefile.linux all
make -f Makefile.linux exe
```

### Windows
To build and run the application on a Windows system:
```sh
cd <Project>
make -f Makefile.windows all
make -f Makefile.windows exe
```

### Wine
To cross-compile for Windows using Wine:
```sh
cd <Project>
make -f Makefile.wine all
make -f Makefile.wine exe
```

### Webassembly
To compile for the web using Emscripten:
```sh
cd <Project>
emmake make -f Makefile.web all
emmake make -f Makefile.web exe
```

For clean builds and other options, refer to the build steps provided above.