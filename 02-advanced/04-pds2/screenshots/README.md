# PDS2 – Visual Evidence Manifest

> Visual reference for dataset creation, member uploading, JCL sorting, and validation on z/OS.

---

## Overview

This folder contains screenshots verifying the successful completion of the PDS2 lab. The images document the workflow of uploading local files, configuring JCL with symbolics, managing dataset members, and the final validation sequence.

---

## Image Manifest

-   [cite_start]**01.png:** The `Z87191.SOURCE` dataset populated with the uploaded rock files (`ROCKS1`, `ROCKS2`, `ROCKS3`), ready for processing[cite: 44, 46].
-   **02.png:** The `MERGSORT` JCL script in the editor. [cite_start]Highlights the use of `&SYSUID` symbolics to dynamically point to the `SOURCE` (input) and `OUTPUT` (destination) datasets[cite: 56, 63].
-   [cite_start]**03.png:** Verification of the `ROCKSOUT` member content, confirming the sort utility successfully merged and alphabetized the rock lists (from "Amphibolite" to "Granodiorite")[cite: 151].
-   [cite_start]**04.png:** The `Z87191.OUTPUT` dataset view showing the member successfully renamed from `ROCKSOUT` to `PDS2OUT` as per challenge requirements[cite: 152].
-   **05.png:** The cleanup step. [cite_start]Displays the confirmation dialog for deleting the temporary `Z87191.PDS2.PUMPKIN` dataset[cite: 161].
-   **06.png:** The "JOBS" panel confirmation. [cite_start]Displays the successful execution of `MERGSORT` (CC 0000) and the final validation job `@APDS2` (CC 0000)[cite: 162].

---

## Contact

For any questions or feedback, reach out:
**Paarth Pandey**
[LinkedIn](https://www.linkedin.com/in/paarth-pandey-13779529b/) | [GitHub](https://github.com/paarthpandey10) | paarthdxb@gmail.com

---

> Author: [Paarth Pandey](https://github.com/paarthpandey10)
>
> IBM Z Xplore - Advanced
