# OS Assignment 2: Process Management and Development Fundamentals

This project provides the solution and necessary files for Assignment 2, focusing on foundational C development concepts within an operating systems context. This includes process creation using `fork()`, understanding the roles of the linker and loader, and automating compilation with a Makefile.

## 📂 Project Contents

The repository is structured as follows:

* `/c_files`: Contains all C source code examples and solutions for the assignment (corresponding to Lab 5 exercises).
* `answers.txt`: Detailed, written explanations addressing all specific assignment questions.
* `Makefile`: The build automation script used to compile, run, and clean the programs.
* `README.md` (This file): Documentation and instructions for the project.
* `LICENSE`: The MIT License file for this project.
* `/screenshots`: Contains visual proof of compilation, execution, and the output of the `ldd` command for shared library analysis.

## 🚀 How to Compile and Run Programs

All build and execution tasks are managed via the provided `Makefile`. Execute all commands from the root directory of the project.

### 1. Compile All Programs

This command uses the `Makefile` to invoke the C compiler (`gcc`) on all necessary source files and create the executable programs.

```bash
make
```

### 2. Run the Programs

Once compiled, you can execute the programs directly. The example programs demonstrate core concepts like process creation.

```bash
./process_creation
./output_program
./simple_program
```

### 3. Test Loader Behavior (Shared Libraries)

Use the `ldd` command (List Dynamic Dependencies) on an executable (like `simple_program`) to see which shared libraries the program needs to load at runtime. This visually demonstrates the Loader's role.

```bash
ldd simple_program
```

### 4. Clean All Compiled Files

Use the `clean` target in the Makefile to remove all generated executable binaries and object files, returning the directory to its initial state.

```bash
make clean
```

## ⚖️ License

This project is licensed under the MIT License.

---

**Note**: Ensure you have `gcc` and `make` installed on your system before attempting to compile the programs. On most Linux distributions, these tools are available through the standard package manager.