# ASM1: Introduction to Assembler Programming

> Building and executing a native Assembler program on z/OS to generate the Fibonacci sequence.

---

## Overview

This module documents the **ASM1** challenge, the entry point into the Advanced IBM Z Xplore badge. The challenge demystifies the compilation process by taking a raw Assembler source file (`fibonacci.s`) and transforming it into an executable program. The goal was to produce a program that calculates and displays the first 38 numbers of the Fibonacci sequence using native machine instructions.

---

## Key Highlights

-   **The compilation Process:**
    -   Used the `as` command to assemble the source code into a binary object file (`fibonacci.o`).
    -   Used the `ld` command to link the object file with system libraries to create the final executable (`fibonacci`).
-   **Assembler Logic:**
    -   **Looping:** The code utilizes the `BCT` (Branch on Count) instruction to loop 38 times, decrementing a counter in Register 5.
    -   **Data Movement:** Leveraged `MVI` and `MVC` instructions to move data and format characters within memory.
    -   **Output:** Since Assembler has no native "print" function, the program calls the `BPX1WRT` service to write results to standard output (stdout).
-   **Linkage Conventions:**
    -   The code establishes "standard linkage," a convention allowing the shell to hand control to the program and receive it back upon completion.

---

## Technical Details

-   **Language:** Assembler (HLASM)
-   **Environment:** z/OS UNIX System Services (USS)
-   **Validation Job:** `ZXP.PUBLIC.JCL(CHKASM1)`
-   **Key Commands:**
    -   `as -o fibonacci.o fibonacci.s`
    -   `ld -o fibonacci fibonacci.o`
    -   `./fibonacci`

---

## Contact

For any questions or feedback, reach out:
**Paarth Pandey**
[LinkedIn](https://www.linkedin.com/in/paarth-pandey-13779529b/) | [GitHub](https://github.com/paarthpandey10) | paarthdxb@gmail.com

---

> Author: [Paarth Pandey](https://github.com/paarthpandey10)
>
> IBM Z Xplore - Advanced
