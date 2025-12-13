# FILES1: Dataset & Member Management

> Mastering Partitioned Data Sets (PDS) and Sequential Files using Zowe Explorer.

---

## Overview

This module documents the **FILES1** challenge of the IBM Z Xplore series. The focus shifts from basic connectivity to active data management. The goal was to perform essential Mainframe operations—creating, renaming, copying, and deleting dataset members—directly within the VS Code interface, bypassing the need for ISPF/green screen panels.

This lab demonstrates how modern tooling can handle legacy file structures (PDS and Sequential Data Sets) efficiently.

---

## Key Highlights

- **Workspace Setup:** Created a custom filter to view `ZXP.PUBLIC` and personal `Z#####` datasets simultaneously.
- **Environment Initialization:** Submitted the `PDSBUILD` JCL job to generate the necessary datasets and members for the challenge.
- **Member Operations:**
  - **Renaming:** Renamed member `M6` to `VIOLET` inside the `INPUT` dataset.
  - **Deletion:** Removed member `M2` to clean up the dataset.
  - **Copy & Paste:** Copied member `RED` from the `SURPRISE` dataset and pasted it into the `INPUT` dataset.
  - **Creation:** Created a completely new member named `MYNEWMBR`.
- **Sequential Files:** Edited `Z87191.SEQDS` to add personal text data.
- **Validation:** Submitted the `@FILES1` job to verify all changes were performed correctly.

---

## Technical Details

- **Setup Job:** `ZXP.PUBLIC.JCL(PDSBUILD)`
- **Validation Job:** `ZXP.PUBLIC.JCL(@FILES1)`
- **Datasets Modified:**
  - `Z87191.INPUT` (PDS)
  - `Z87191.SURPRISE` (PDS)
  - `Z87191.SEQDS` (Sequential)
- **Tools:** Zowe Explorer, IBM Z Open Editor

---

## Contact

For any questions or feedback, reach out:
**Paarth Pandey** [LinkedIn](https://www.linkedin.com/in/paarth-pandey-13779529b/) | [GitHub](https://github.com/paarthpandey10) | paarthdxb@gmail.com

---

> Author: [Paarth Pandey](https://github.com/paarthpandey10)
>
> IBM Z Xplore - Fundamentals
