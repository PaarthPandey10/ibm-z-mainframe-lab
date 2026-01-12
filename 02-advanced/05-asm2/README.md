# ASM2: Developers Assemble!

> Introduction to IBM Z Assembler language, TSO TEST facility, and source code modification.

---

## Overview

This module documents the **ASM2** challenge, which provides a practical introduction to the High Level Assembler (HLASM) on z/OS. The challenge involves understanding existing Assembler logic, using the TSO TEST facility to inspect program execution, and modifying source code to alter program behavior, specific registers, and logic flow.

---

## Key Highlights

-   **Code Analysis & Setup:**
    -   **Replication:** Copied the public `ASMPGM` source member to a private dataset as `ASM2PGM` to establish a working baseline.
    -   **JCL Configuration:** Updated the JCL compilation target to output a new load module named `ASM2PGM`.
-   **Logic Modification:**
    -   **Register Swapping:** Modified the source code to replace all instances of Register 2 with Register 6 and Register 3 with Register 7 to demonstrate control over processor resources.
    -   **Algorithm Updates:** Altered the loop logic to execute 10 times (previously 4) and increment the summation register by 5 (previously 1) during each iteration.
-   **Execution & Validation:**
    -   **Compilation:** Successfully compiled and linked the modified Assembler program using the `ASMACL` procedure.
    -   **Verification:** Validated the logic changes and register usage using the `CHKASM2` automated checker.

---

## Technical Details

-   **System:** IBM z/OS via Zowe Explorer
-   **Language:** IBM High Level Assembler (HLASM)
-   **Key Files:**
    -   `ASM2PGM` (Modified Source Code & JCL)
    -   `CHKASM2` (Validation JCL)
-   **Validation:** Job `ASM2PGM` ended with `CC 0000`, followed by successful `@ASM2` (CHKASM2) verification.

---

## Contact

For any questions or feedback, reach out:
**Paarth Pandey**
[LinkedIn](https://www.linkedin.com/in/paarth-pandey-13779529b/) | [GitHub](https://github.com/paarthpandey10) | paarthdxb@gmail.com

---

> Author: [Paarth Pandey](https://github.com/paarthpandey10)
>
> IBM Z Xplore - Advanced
