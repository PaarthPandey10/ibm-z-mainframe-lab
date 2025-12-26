# REXX1 – Zowe CLI & TSO Screenshots

> Visual reference for Zowe CLI installation, file management, and interactive REXX execution performed during the REXX1 challenge.

---

## Overview

This folder contains screenshots verifying the successful completion of the REXX1 lab.
The images document the workflow of setting up the Zowe environment on Windows and using it to play the `GUESSNUM` game via a TSO address space.

---

## Image Manifest

- **01.png:** Installing the Zowe CLI using `npm i -g @zowe/cli` in the Windows command prompt.
- **02.png:** Zowe Explorer view showing `SOMEREXX` and `GUESSNUM` successfully copied to `Z87191.SOURCE`.
- **03.png:** Validating the Zowe connection with `files list ds` and running `SOMEREXX` to see the "GREETINGS FROM REXX" output.
- **04.png:** The interactive `GUESSNUM` session using `zowe tso send as` to submit guesses (1, 2, 5, 3, 4) to the active address space.
- **05.png:** Zowe Explorer "JOBS" view confirming the `@REXX1` validation job ended with `CC 0000`.

---

## Contact

For any questions or feedback, reach out:
**Paarth Pandey**
[LinkedIn](https://www.linkedin.com/in/paarth-pandey-13779529b/) | [GitHub](https://github.com/paarthpandey10) | paarthdxb@gmail.com

---

> Author: [Paarth Pandey](https://github.com/paarthpandey10)
>
> IBM Z Xplore - Fundamentals
