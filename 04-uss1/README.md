# USS1: UNIX System Services

> Navigating the UNIX environment within z/OS, executing shell scripts, and managing file I/O redirection.

---

## Overview

This module documents the **USS1** challenge of the IBM Z Xplore series. Unlike previous JCL-focused challenges, this lab introduces **UNIX System Services (USS)**, a POSIX-compliant environment embedded within z/OS. The goal was to master command-line navigation, execute shell scripts (like `scramble.sh`), and utilize standard UNIX I/O redirection to decode hidden messages.

This lab demonstrates that z/OS is a hybrid environment, allowing users to interact via standard UNIX commands (`ls`, `cd`, `grep`) while retaining access to mainframe datasets.

---

## Key Highlights

- **Environment Access:**
  - [cite_start]Connected to the mainframe using **SSH** (Secure Shell) via VS Code terminal[cite: 71, 72].
  - [cite_start]Initialized the workspace using the `uss-setup` command to populate the home directory[cite: 108].
- **File System Navigation:**
  - [cite_start]Navigated the hierarchical directory structure using `cd`, `ls`, and `pwd`[cite: 137, 151].
  - [cite_start]Created and managed files using `touch` (create file), `mkdir` (create directory), and `rm` (remove)[cite: 204, 205, 272].
- **Script Execution & Decoding:**
  - [cite_start]Executed a shell script `./scramble.sh` to decode a secret message located at `/z/public/secret.txt`[cite: 256].
  - [cite_start]Solved a "Caesar cipher" style rotation puzzle by determining the correct rotation argument[cite: 250, 265].
- **I/O Redirection:**
  - [cite_start]Redirected standard output (`stdout`) to a file using `>` to save the decoded message[cite: 297, 302].
  - [cite_start]Appended system information (`du -ak` and `date`) to the same file using `>>` to create a comprehensive log[cite: 317, 348].
- **Validation:**
  - [cite_start]Submitted the `CHKUSS1` job to verify the contents of `ussout.txt`[cite: 375].

---

## Technical Details

- **Setup Command:** `uss-setup`
- **Validation Job:** `ZXP.PUBLIC.JCL(CHKUSS1)`
- **Key Concepts:**
  - **USS (UNIX System Services):** Running UNIX workloads on IBM Z.
  - **Redirection:** Using `>` (overwrite) and `>>` (append).
  - [cite_start]**Permissions:** Understanding executable bits (`x`) in file listings (`ls -l`)[cite: 239].
  - [cite_start]**Zowe Integration:** Viewing USS hierarchies via the Zowe Explorer VS Code extension[cite: 213].
- **Tools:** VS Code Terminal, OpenSSH, Zowe Explorer.

---

## Contact

For any questions or feedback, reach out:
**Paarth Pandey**
[LinkedIn](https://www.linkedin.com/in/paarth-pandey-13779529b/) | [GitHub](https://github.com/paarthpandey10) | paarthdxb@gmail.com

---

> Author: [Paarth Pandey](https://github.com/paarthpandey10)
>
> IBM Z Xplore - Fundamentals