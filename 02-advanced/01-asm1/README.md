# ASM1: Introduction to Assembler Programming

> Building and executing a native Assembler program on z/OS to generate the Fibonacci sequence.

---

## Overview

This module documents the **ASM1** challenge, the entry point into the Advanced IBM Z Xplore badge. [cite_start]The challenge demystifies the compilation process by taking a raw Assembler source file (`fibonacci.s`) and transforming it into an executable program[cite: 201]. [cite_start]The goal was to produce a program that calculates and displays the first 38 numbers of the Fibonacci sequence using native machine instructions[cite: 54].

---

## Key Highlights

-   **The compilation Process:**
    -   [cite_start]Used the `as` command to assemble the source code into a binary object file (`fibonacci.o`)[cite: 206, 207].
    -   [cite_start]Used the `ld` command to link the object file with system libraries to create the final executable (`fibonacci`)[cite: 210, 211].
-   **Assembler Logic:**
    -   [cite_start]**Looping:** The code utilizes the `BCT` (Branch on Count) instruction to loop 38 times, decrementing a counter in Register 5[cite: 153].
    -   [cite_start]**Data Movement:** Leveraged `MVI` and `MVC` instructions to move data and format characters within memory[cite: 149, 150].
    -   [cite_start]**Output:** Since Assembler has no native "print" function, the program calls the `BPX1WRT` service to write results to standard output (stdout)[cite: 191, 192].
-   **Linkage Conventions:**
    -   [cite_start]The code establishes "standard linkage," a convention allowing the shell to hand control to the program and receive it back upon completion[cite: 102].

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
