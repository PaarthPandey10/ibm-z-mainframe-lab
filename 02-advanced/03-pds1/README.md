# PDS1: Get Comfy with Datasets and Members

> Managing Partitioned Data Sets (PDS), copying members, and executing JCL to manipulate datasets on z/OS.

---

## Overview

This module documents the **PDS1** challenge, which moves beyond basic file viewing to active dataset management. The challenge involves understanding the structure of Partitioned Data Sets (PDS), using High Level Qualifiers (HLQ) to filter views, copying members between public and private datasets, and executing JCL to generate specific outputs.

---

## Key Highlights

-   **Dataset Organization:**
    -   **Filtering:** Utilized High Level Qualifiers (HLQ) in Zowe Explorer to switch views between personal datasets (`Z87191.*`) and public resources (`ZXP.PUBLIC.*`).
    -   **Attribute Inspection:** Analyzed dataset attributes (such as Volume Serial `VPWRKD`) to understand physical storage locations on the mainframe.
-   **Member Management:**
    -   **Replication:** Successfully copied required members (`PDSPART1`, `PDSPART2`) from the public input library into the personal `SOURCE` dataset.
    -   **Renaming:** Renamed the generated output member `PDS1OUT` to `RECIPE` to meet the challenge's logical requirements.
-   **Job Execution:**
    -   **JCL Submission:** Submitted the `PDS1CCAT` job, which processed the source members and concatenated them to create a new output member.

---

## Technical Details

-   **System:** IBM z/OS via Zowe Explorer
-   **Data Structure:** Partitioned Data Sets (PDS/PDSE)
-   **Key Files:**
    -   `PDSPART1` & `PDSPART2` (Source Inputs)
    -   `PDS1CCAT` (JCL for Concatenation)
    -   `RECIPE` (Final Renamed Output)
-   **Validation:** Job ended with `CC 0000` (Condition Code Success).

---

## Contact

For any questions or feedback, reach out:
**Paarth Pandey**
[LinkedIn](https://www.linkedin.com/in/paarth-pandey-13779529b/) | [GitHub](https://github.com/paarthpandey10) | paarthdxb@gmail.com

---

> Author: [Paarth Pandey](https://github.com/paarthpandey10)
>
> IBM Z Xplore - Advanced
