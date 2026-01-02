# WRAPUP: Z Open Automation Utilities (ZOAU)

> Automating z/OS system administration tasks using Python and the ZOAU library.

---

## Overview

This module documents the **WRAPUP** challenge, the final lab of the IBM Z Xplore Fundamentals series. This challenge focuses on **Z Open Automation Utilities (ZOAU)**, a set of tools that allows developers to perform native z/OS tasks—like dataset manipulation and system querying—using modern scripting languages like Python. The objective was to write a Python script that generates a report of the system's "Linklist" libraries.

---

## Key Highlights

- **Command Line Utilities:**
  - Used `decho` with the `-a` (append) flag to add text to the bottom of a sequential dataset directly from the UNIX shell.
- **Python Integration:**
  - Utilized the `zoautil_py` library to interact with the mainframe file system.
  - Ran `dslist.py` to programmatically list members of a Partitioned Data Set (PDS).
- **Script Development (`members.py`):**
  - **Dynamic Creation:** Modified the script to create a new Sequential (`SEQ`) dataset named `COMPLETE` if it didn't already exist.
  - **System Query:** Used `zsystem.list_linklist()` to capture the active Linklist (the set of libraries loaded at startup).
  - **File I/O:** Wrote the captured Linklist data into the new dataset using `datasets.write()`.
- **Validation:**
  - Successfully executed the script and submitted the `@AUTO` job to verify the contents of `Z87191.COMPLETE`.

---

## Technical Details

- **Language:** Python 3
- **Libraries:** `zoautil_py` (`datasets`, `zsystem`)
- **Validation Job:** `ZXP.PUBLIC.JCL(CHKAUTO)` (Alias: `@AUTO`)
- **Key Functions:**
  - `datasets.create(name, dataset_type="SEQ")`.
  - `zsystem.list_linklist()`.
  - `datasets.write(name, content, append=False)`.

---

## Contact

For any questions or feedback, reach out:
**Paarth Pandey**
[LinkedIn](https://www.linkedin.com/in/paarth-pandey-13779529b/) | [GitHub](https://github.com/paarthpandey10) | paarthdxb@gmail.com

---

> Author: [Paarth Pandey](https://github.com/paarthpandey10)
>
> IBM Z Xplore - Fundamentals
