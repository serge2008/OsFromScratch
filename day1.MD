# Day 1: Setting Up the Environment

Today, I began creating the project and setting up the environment. I was working on `Windows`, so I had to install MSYS2. I got it from here:
- [MSYS2 Official Website](https://www.msys2.org/)

### Steps Taken:
1. **Downloaded and Installed MSYS2**:
   - Followed the installation instructions on the website.
   - Configured the environment by updating the package database and installing essential tools like `gcc`, `make`, and `qemu`.

2. **Started a Git Repository**:
   - Created the **.gitignore** file:
     ```plaintext
     *.log
     /.vscode/
     ```

3. **Set Up the Directory Structure**:
   - Created the following directories:
     ```plaintext
     OSFromScratch/
     ├── Preliminary
         ├── C/
         ├── Day1Continued.MD
         └── Assembly/
     ├── Bootloader/placeholder
     ├── Kernel/placeholder
     ├── GraphicsLibrary/placeholder
     ├── Day1.MD
     ├── README.MD
     ├── .gitignore
     └── tree.log
     ```

4. **Tested the Setup**:
   - Wrote and compiled a simple "Hello World" program in C to confirm everything was working correctly (not included in the log).

### Challenges:
- **Cross-compiler Setup**:
  - Learned about the importance of a cross-compiler for OS development. I started looking into resources to set up a GCC cross-compiler. A useful reference is [OSDev Wiki](https://wiki.osdev.org/GCC_Cross-Compiler).

### Next Steps:
- Begin learning preliminary topics (C and assembly basics).
- Complete the cross-compiler setup.
- Write a basic bootloader to test the build environment.
- Start documenting the bootloader code.

---

continued: **[Day 1 Continued Part 1](preliminary/Day1continued.MD)**
