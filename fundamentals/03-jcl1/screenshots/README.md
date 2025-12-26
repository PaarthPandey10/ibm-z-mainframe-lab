# JCL1 – Job Control & Execution Screenshots

> Visual reference for key debugging and execution steps performed during the JCL1 challenge.

---

## Overview

This folder contains screenshots verifying the successful completion of the JCL1 lab.
The images document the lifecycle of job submission, error identification (CC 0012/Abends), and the code corrections required for `IEBGENER` and COBOL compilation.

---

## Image Manifest

- **01.png:** Submitting the initial `JCLSETUP` job to allocate datasets.
- **02.png:** Verifying the `JCLSETUP` job completed with **CC 0000**.
- **03.jpg:** Composite view showing the workflow of submitting jobs and viewing output side-by-side.
- **04.png:** Editing `JCL1` to fix the `IEBGENER` copy step (correcting DSN references).
- **05.png:** Debugging `JCL2`: Fixing the DD Name (`//COMBINED`) to match the COBOL source code.
- **06.png:** Editing `JCL3` to format in-stream data for the train schedule output.

---

## Contact

For any questions or feedback, reach out:
**Paarth Pandey**
[LinkedIn](https://www.linkedin.com/in/paarth-pandey-13779529b/) | [GitHub](https://github.com/paarthpandey10) | paarthdxb@gmail.com

---

> Author: [Paarth Pandey](https://github.com/paarthpandey10)
>
> IBM Z Xplore - Fundamentals
