# IBM Z Xplore: Advanced

> Diving deeper into system architecture, Assembler programming, and low-level z/OS operations.

---

## About

This directory documents the **Advanced** phase of my IBM Z Xplore journey. While the Fundamentals module focused on bridging modern tools with the mainframe, this module shifts focus to the underlying architecture.

The objective is to peel back the layers of high-level languages and understand how the machine actually processes instructions. [cite_start]This involves working directly with **Assembler**, understanding memory management, registers, and the compilation process on z/Architecture[cite: 32, 44].

---

## Project Structure

| Directory | Challenge | Description | Key Technologies |
| :--- | :--- | :--- | :--- |
| **[`01-asm1`](./01-asm1)** | **Assembler Intro** | Compiling, linking, and running an Assembler program to calculate Fibonacci numbers. | HLASM, Linker (`ld`), USS, Registers |
| *[Upcoming]* | *...* | *Future advanced challenges (REXX, JCL, etc.)* | *...* |

---

## Features / Highlights

-   [cite_start]**Low-Level Control:** Moving away from abstractions to understand how **Assembler** manipulates hardware directly for high-security and real-time performance[cite: 46, 48].
-   [cite_start]**Compilation Pipeline:** Manually managing the build process: converting Source Code (`.s`) $\to$ Object File (`.o`) $\to$ Executable Binary[cite: 207, 208].
-   **System Services:** Interfacing directly with z/OS UNIX System Services (USS) to execute binary programs.

---

## Technologies Used

-   **Operating System:** z/OS (UNIX System Services)
-   **Languages:** High Level Assembler (HLASM)
-   **Tools:** VS Code, Terminal (SSH)
-   **System Utilities:** `as` (Assembler), `ld` (Linker), `BPX1WRT` (Output Service)

---

## Contact

**Paarth Pandey**
[LinkedIn](https://www.linkedin.com/in/paarth-pandey-13779529b/) | [GitHub](https://github.com/paarthpandey10) | paarthdxb@gmail.com

---

> Author: [Paarth Pandey](https://github.com/paarthpandey10)
>
> IBM Z Xplore: Advanced
