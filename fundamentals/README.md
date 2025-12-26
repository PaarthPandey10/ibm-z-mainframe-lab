# IBM Z Xplore: Fundamentals

> Mastering connectivity, data set management, and system automation on z/OS using modern open-source tools.

---

## About

This directory documents the **Fundamentals** phase of my IBM Z Xplore journey. The primary objective of this module was to bridge the gap between traditional mainframe operations and modern development workflows.

Through these seven challenges, I moved from establishing basic connectivity to developing complex automation scripts that leverage the hybrid nature of z/OS—combining traditional MVS Data Sets with UNIX System Services (USS) and Python.

---

## Project Structure

| Directory | Challenge | Description | Key Technologies |
| :--- | :--- | :--- | :--- |
| **[`01-vsc1`](./01-vsc1)** | **VS Code Setup** | Establishing a connection to the IBM Z mainframe using modern IDEs. | VS Code, Zowe Explorer |
| **[`02-files1`](./02-files1)** | **Data Sets** | Understanding z/OS file systems, creating PDS members, and editing data. | Partitioned Data Sets (PDS) |
| **[`03-jcl1`](./03-jcl1)** | **JCL Basics** | Writing and submitting Job Control Language (JCL) to execute system tasks. | JCL, JOB, EXEC, DD |
| **[`04-uss1`](./04-uss1)** | **UNIX** | Navigating the POSIX-compliant UNIX shell within z/OS. | SSH, Shell Scripting, I/O Redirection |
| **[`05-code1`](./05-code1)** | **Python Intro** | Running Python workloads natively on z/OS to handle logic and math. | Python 3, String Manipulation |
| **[`06-rexx1`](./06-rexx1)** | **REXX & CLI** | Using the Zowe CLI and TSO Address Spaces for interactive scripting. | REXX, Zowe CLI, TSO |
| **[`07-wrapup`](./07-wrapup)** | **Automation** | Combining Python with ZOAU to automate system administration tasks. | ZOAU, `zoautil_py`, System Automation |

---

## Features / Highlights

-   **Modern Connectivity:** Abandoned legacy "Green Screen" emulators in favor of **VS Code** and the **Zowe Explorer** extension for a modern IDE experience.
-   **Hybrid Architecture:** Demonstrated proficiency in managing both traditional **MVS Data Sets** and hierarchical **UNIX (USS)** files.
-   **Multi-Language Scripting:** Executed workloads using **JCL** (Job Control Language), **Python 3**, and **REXX**.
-   **System Automation:** Utilized **ZOAU** (Z Open Automation Utilities) to programmatically query system Linklists and dynamically create data sets without manual intervention.

---

## Technologies Used

-   **Operating System:** z/OS
-   **Languages:** Python 3, REXX, JCL, Shell (Bash/Zsh)
-   **Tools:** VS Code, Zowe Explorer, Zowe CLI, NPM
-   **Libraries:** `zoautil_py` (Python for z/OS), `datasets`, `zsystem`

---

## Contact

**Paarth Pandey**
[LinkedIn](https://www.linkedin.com/in/paarth-pandey-13779529b/) | [GitHub](https://github.com/paarthpandey10) | paarthdxb@gmail.com

---

> Author: [Paarth Pandey](https://github.com/paarthpandey10)
>
> IBM Z Xplore: Fundamentals
