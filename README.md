# OOP Lab Work 01: GCD C++ Program

### Lab Work №1 from MAI OOP course 

## Goal

* Study C++ build systems using CMake
* Study version control systems Git
* Study memory management in C++
* Study input/output operations to the standard stream
* Study unit testing using the Google Test Framework

## Project Structure

```
GCD/
├── CMakeLists.txt          # CMake configuration file
├── main.cpp                # Main program
├── README.md               # This file
├── include/
│   └── GCD.hpp             # Header file with function declarations
├── src/
│   └── GCD.cpp             # Function implementations
├── tests/
│   └── test01.cpp          # Unit tests using Google Test
└── build/                  # Build directory (generated)
    ├── bin/                # Compiled executables
    └── lib/                # Compiled libraries
```

## Installation Instructions

### Installing a C++ Compiler

Download and install the latest version of C++:

* **Windows**: it is recommended to use [MinGW-w64](https://www.mingw-w64.org/downloads/) or Visual Studio Community
* **macOS**: it is recommended to install "Xcode" and "Xcode Command Line Tools" from [developer.apple.com](https://developer.apple.com/xcode/)
* **Linux** (gcc version 12 or higher recommended):
  ```bash
  sudo apt update
  sudo apt install build-essential
  ```

### Installing CMake

Download and install the latest version of CMake from [cmake.org](https://cmake.org/download/)

### Installing Git

Download and install the latest version of Git for your operating system from [git-scm.com](https://git-scm.com/downloads)


## Building and Running the Project

### Building the Project

```bash
# Create a build directory
mkdir build
cd build

# Configure the project
cmake ..

# Build the project
cmake --build .
```

### Running the Main Program

```bash
# From the build directory
./Lab01_exe
```

### Running the Tests

```bash
# From the build directory
./tests

# Or via CTest
ctest --verbose
```