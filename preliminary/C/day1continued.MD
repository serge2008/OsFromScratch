# Day 1 Continued: Exploring C

## Introduction
Today, I focused on diving deeper into C programming as part of the preliminary steps for building my custom OS. The goal is to solidify the foundation of C before tackling assembly and kernel development.

### Key Learnings
1. **Basic C Syntax**:
   - Variables and Data Types
   - Functions and Control Flow (If-Else, Loops)
   - Arrays and Pointers

2. **Compiling and Debugging**:
   - Learned how to compile a simple C program using `gcc`.
   - Used debugging tools like `gdb` to inspect and trace the execution of code.

## Code Example: Hello World Program

```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```
## Steps Taken:
1. **Compiling and Testing the "Hello World" Program**:
   - After writing the code, I compiled it using the `gcc` command:
     ```bash
     gcc hello.c -o hello
     ```
   - I then executed the program:
     ```bash
     ./hello
     ```
   - The output displayed as expected:
     ```
     Hello, World!
     ```
   This confirmed that the environment and compiler were correctly set up.

2. **Learning to Use `gdb` for Debugging**:
   - I learned how to run the program with `gdb` to trace the execution and examine variables:
     ```bash
     gdb ./hello
     ```
   - I set breakpoints, inspected variable values, and walked through the program’s execution to understand how it works at a low level.

3. **Familiarizing with Pointers and Memory Management**:
   - Today, I worked on understanding the basics of pointers in C, including pointer arithmetic and dereferencing. I wrote a simple program to manipulate and print the value of a variable through a pointer:
     ```c
     #include <stdio.h>

     int main() {
         int num = 10;
         int *ptr = &num;

         printf("Value of num: %d\n", num);
         printf("Value through pointer: %d\n", *ptr);
         return 0;
     }
     ```
   - Output:
     ```
     Value of num: 10
     Value through pointer: 10
     ```
4. **Update gitignore**
  - i updated gitignore to inclode more files:
    ```.gitignore
    # Ignore system files
    Thumbs.db
    Desktop.ini
    $RECYCLE.BIN/

    # Ignore IDE or editor-specific files
    .vscode/
    .idea/

    # Ignore compiled code
    *.exe
    *.out
    *.o
    *.a
    *.so
    *.dll

    # Ignore backup files
    *~
    *.bak
    *.swp
    *.swo

    # Ignore logs
    *.log

    # Ignore temporary files
    *.tmp
    *.temp

    # Ignore MSYS2 specific files (e.g., package management and config)
    /mingw64/
    /msys64/
    /usr/

    ```
### Challenges:
- **Pointer Arithmetic**: It was initially challenging to understand pointer arithmetic and memory management. I had to review resources multiple times to gain clarity.
- **Debugging with `gdb`**: Learning how to properly use `gdb` was somewhat tricky, but with practice, I got the hang of setting breakpoints and stepping through the code.

## Next Steps:
- Practice more pointer-related tasks, as they are crucial for interacting with memory in C.
- Start exploring more complex topics, like structures, dynamic memory allocation, and file I/O.
- Begin looking into assembly language and its integration with C for OS development.

