# ASM2 – Visual Evidence Manifest

> Visual reference for Assembler source modification, JCL configuration, and successful validation on z/OS.

---

## Overview

This folder contains screenshots verifying the successful completion of the ASM2 lab. The images document the workflow of modifying Assembler registers and loop logic, configuring the build JCL, and verifying the final condition codes.

---

## Image Manifest

-   **01.png:** The `Z87191.SOURCE(ASM2PGM)` member showing the base Assembly code structure before final logic updates.
-   **02.png:** The modified source logic. Highlights the specific changes: utilizing Register 6 and 7, setting the loop count to 10 (`F'10'`), and the increment value to 5 (`F'5'`).
-   **03.png:** The `Z87191.JCL` dataset view confirming the creation of the `ASM2PGM` JCL member.
-   **04.png:** The JCL configuration view. Shows the update to the `EXEC` statement (`MBR=ASM2PGM`) and the integration of the source code within the job stream.
-   **05.png:** The "JOBS" panel confirming the successful compilation and execution of the `ASM2PGM` job with Return Code `CC 0000`.
-   **06.png:** The validation step. Displays the successful execution of the `@ASM2` job (alias for `CHKASM2`) with `CC 0000`, confirming the output matches the challenge requirements.

---

## Contact

For any questions or feedback, reach out:
**Paarth Pandey**
[LinkedIn](https://www.linkedin.com/in/paarth-pandey-13779529b/) | [GitHub](https://github.com/paarthpandey10) | paarthdxb@gmail.com

---

> Author: [Paarth Pandey](https://github.com/paarthpandey10)
>
> IBM Z Xplore - Advanced
