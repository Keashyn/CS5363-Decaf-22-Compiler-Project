# CS5363-Decaf-22-Compiler-Project

This project is a compiler for the Decaf Programming Language. The compiler consists of several
phases: 
* Lexer
* Parser
* type checker
* code generator

The lexer phase takes a Decaf source file as input and generates a stream of token.
The parser phase consumes the stream of tokens and generates an Abstract Syntax Tree (AST)
representing the structure of the program. The type checker phase performs type checking on the
AST and generates type annotations. The code generator phase generates assembly code from the annotated
AST.

# Installation

The Decaf-22 Compiler requires the following dependencies:
* cmake (>=3.26.0)

To build the project, run the following command from the project root directory:
```bash
./workdir/build.sh
```
Then run the following command from the project root directory:
```bash
./workdir/exec.sh
```

# Usage
Use the provide execution script to run, expects source file as parameter and outputs all information to stdout, can use redirection to write to file
```
# Run with output on stdout
./workdir/exec.sh <source_file>

# Run and save output to file
./workdir/exec.sh <source_file> > <output_file>

# Run binary directly with output on stdout
./decaf-22 <source_file>
```

# Project Structure

* **CmakeLists.txt** : This file is used to build the project using CMake, a cross-platform build system. It is used through out the entire Decaf 22 Compiler project. 

* **src** : This directory contains source code and sub-folder for each file such as **lexer** and **token** for the
Decaf 22 Compiler and include the **main.cpp** file as well.

* **include** : This directory contains the header files for the Decaf 22 compiler and includes the declarations of classes,
functions and data structure used in the compiler.

* **workdir** : This directory is used to store the temporary files generated during the build process, as well as the output files generated after the compilation. It contains two bash files which are **build.sh** and **exec.sh** to run the
Decaf 22 compiler project.

* **dependencies** : This directory contains the external dependencies required by the Decaff 22 compiler. It includes the libraries, headers and other resources required for the compiler to work correctly.

* **tests** : This directory contains the unit tests for the Decaff 22 compiler. It includes the code for testing the different functionalities of the compiler, as well as the test data used for validation

# Author and Acknowledgement
* Keashyn Naidoo (Sif274)

# License

This project is licensed under the MIT License - see the [LICENSE.md] file for details.