# PDS1 – Dataset Management Screenshots

> Visual reference for PDS manipulation, member copying, and JCL job validation on z/OS.

---

## Overview

This folder contains screenshots verifying the successful completion of the PDS1 lab. The images document the workflow of filtering datasets, managing members via the Zowe Explorer GUI, and validating the job completion status.

---

## Image Manifest

-   **01.png:** The initial environment setup in Zowe Explorer. displays the Data Sets view filtered by the user HLQ (`Z87191`), showing the `JCL` and `SOURCE` Partitioned Data Sets ready for population.
-   **02.png:** A detailed view of the workspace after main operations. It highlights the `Z87191.SOURCE` dataset containing the copied members (`PDSPART1`, `PDSPART2`) and the final renamed member (`RECIPE`). It also shows the Attributes panel for `ZXP.PUBLIC.INPUT`, verifying the Volume Serial `VPWRKD`.
-   **03.png:** A clean view of the `Z87191.SOURCE` directory structure, confirming that all required members are present and correctly named (`GUESSNUM`, `PDSPART1`, `PDSPART2`, `RECIPE`, `SOMEREXX`).
-   **04.png:** The "JOBS" panel confirmation. Displays the successful execution of the validation job (`@APDS1`) returning a Condition Code of `0000`, signifying the challenge was completed without errors.

---

## Contact

For any questions or feedback, reach out:
**Paarth Pandey**
[LinkedIn](https://www.linkedin.com/in/paarth-pandey-13779529b/) | [GitHub](https://github.com/paarthpandey10) | paarthdxb@gmail.com

---

> Author: [Paarth Pandey](https://github.com/paarthpandey10)
>
> IBM Z Xplore - Advanced
