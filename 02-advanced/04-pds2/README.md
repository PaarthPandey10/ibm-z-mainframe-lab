# PDS2: Advanced Filtering and Editing of Data Sets

> Advanced dataset allocation, member uploads, and JCL symbolic substitution for data processing on z/OS.

---

## Overview

This module documents the **PDS2** challenge, which advances from basic dataset interaction to active creation and management. The challenge focuses on the lifecycle of data on the mainframe: creating new Partitioned Data Sets (PDS), uploading local files to the system, processing them via JCL with symbolic variables, and performing cleanup operations to maintain a hygienic workspace.

---

## Key Highlights

-   **Data Ingestion & Allocation:**
    -   **Allocation:** Created a new Partitioned Data Set (`Z87191.PDS2.PUMPKIN`) to understand allocation parameters and naming conventions.
    -   **Uploading:** Uploaded local text files (`ROCKS1`, `ROCKS2`, `ROCKS3`) directly into the `SOURCE` PDS from the local machine.
-   **JCL & Data Processing:**
    -   **Symbolics:** Utilized the `MERGSORT` JCL which leverages the `&SYSUID` symbolic variable to dynamically reference personal datasets (`SOURCE` and `OUTPUT`).
    -   **Sorting:** Executed a sort operation that merged three distinct members into a single, alphabetized output member (`ROCKSOUT`).
-   **Hygiene & Validation:**
    -   **Renaming:** Renamed the processed output member `ROCKSOUT` to `PDS2OUT` to meet validation criteria.
    -   **Cleanup:** Deleted the temporary dataset (`Z87191.PDS2.PUMPKIN`) to demonstrate proper storage management before final validation.

---

## Technical Details

-   **System:** IBM z/OS via Zowe Explorer
-   **Data Structure:** Partitioned Data Sets (PDS/PDSE)
-   **Key Files:**
    -   `ROCKS1-3` (Uploaded Inputs)
    -   `MERGSORT` (JCL with Sort logic)
    -   `PDS2OUT` (Final Renamed Output)
-   **Validation:** Job `@APDS2` ended with `CC 0000` (Condition Code Success).

---

## Contact

For any questions or feedback, reach out:
**Paarth Pandey**
[LinkedIn](https://www.linkedin.com/in/paarth-pandey-13779529b/) | [GitHub](https://github.com/paarthpandey10) | paarthdxb@gmail.com

---

> Author: [Paarth Pandey](https://github.com/paarthpandey10)
>
> IBM Z Xplore - Advanced
