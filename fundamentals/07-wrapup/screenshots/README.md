# WRAPUP – ZOAU Automation Screenshots

> Visual reference for using `decho`, running ZOAU Python scripts, and validating system automation tasks.

---

## Overview

This folder contains screenshots verifying the successful completion of the WRAPUP lab.
The images document the use of Z Open Automation Utilities to append data to files, list dataset members, and generate a system Linklist report using Python.

---

## Image Manifest

- **01.png:** Setup step showing the `ALLOC` job used to ensure the `JCL3OUT` dataset existed.
- **02.png:** Execution of the `decho` command to append text to `JCL3OUT` and verification using `cat`.
- **03.png:** Output of `dslist.py` showing a programmatic list of PDS members (`JCL1`, `JCL2`, `JCL3`).
- **04.png:** Source code changes in `members.py`, highlighting the `SEQ` dataset type correction and the `list_linklist` function call.
- **05.png:** Final execution of `members.py` creating the `COMPLETE` dataset, followed by the successful `@AUTO` validation job.

---

## Contact

For any questions or feedback, reach out:
**Paarth Pandey**
[LinkedIn](https://www.linkedin.com/in/paarth-pandey-13779529b/) | [GitHub](https://github.com/paarthpandey10) | paarthdxb@gmail.com

---

> Author: [Paarth Pandey](https://github.com/paarthpandey10)
>
> IBM Z Xplore - Fundamentals
