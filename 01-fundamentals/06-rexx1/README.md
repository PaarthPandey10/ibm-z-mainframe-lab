# REXX1: Zowe CLI & REXX Scripting

> Configuring the Zowe Command Line Interface and executing interactive REXX programs on z/OS.

---

## Overview

This module documents the **REXX1** challenge of the IBM Z Xplore series. This challenge introduces **REXX** (Restructured Extended Executor), a scripting language often referred to as "Enterprise IT Duct Tape" due to its versatility. The primary objective was to move beyond the VS Code GUI and install the **Zowe CLI** on the local machine, allowing for direct command-line interaction with the mainframe. The lab concluded with managing TSO address spaces to play an interactive number-guessing game.

---

## Key Highlights

- **Zowe CLI Installation:**
  - Installed the `@zowe/cli` package globally using npm (`Node Package Manager`) on Windows.
  - Configured TSO and z/OSMF profiles to enable secure, password-less communication with the host.
- **Data Set Management:**
  - Copied source members `SOMEREXX` and `GUESSNUM` from `ZXP.PUBLIC.SOURCE` to the personal dataset `Z87191.SOURCE` using Zowe Explorer.
- **REXX Execution:**
  - **Batch Mode:** Ran `SOMEREXX` using `zowe tso issue command`, which produced a static ASCII art greeting.
  - **Interactive Mode:** Ran `GUESSNUM` by starting a TSO Address Space (`zowe tso start as`). This allowed for a back-and-forth session where I sent specific numbers to the running program until I solved the puzzle.
- **Validation:**
  - Submitted the `@REXX1` job to verify the successful completion of the tasks.

---

## Technical Details

- **Language:** REXX (Restructured Extended Executor)
- **Validation Job:** `ZXP.PUBLIC.JCL(CHKREXX1)`
- **Key Commands:**
  - `npm i -g @zowe/cli` (Installation)
  - `zowe tso issue command` (Single execution)
  - `zowe tso start as` (Start Address Space)
  - `zowe tso send as` (Send input to Address Space)
- **Key Concepts:**
  - **TSO (Time Sharing Option):** The command-line interface for z/OS.
  - **Address Space:** A block of memory allocated for running programs; required for keeping an interactive session "alive".

---

## Contact

For any questions or feedback, reach out:
**Paarth Pandey**
[LinkedIn](https://www.linkedin.com/in/paarth-pandey-13779529b/) | [GitHub](https://github.com/paarthpandey10) | paarthdxb@gmail.com

---

> Author: [Paarth Pandey](https://github.com/paarthpandey10)
>
> IBM Z Xplore - Fundamentals
