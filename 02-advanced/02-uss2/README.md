# USS2: Shell Scripting on z/OS

> Debugging, configuring, and executing a UNIX Shell Script to automate file operations on z/OS.

---

## Overview

This module documents the **USS2** challenge, which focuses on advanced interaction with z/OS UNIX System Services (USS). The challenge requires analyzing a pre-written shell script (`animals.sh`), identifying missing dependencies (directories and files), modifying file permissions, and executing the script with arguments to trigger a successful completion message.

---

## Key Highlights

-   **Script Analysis:**
    -   **Conditional Logic:** Analyzed the script's `if` statements to understand the prerequisites: the existence of a specific directory (`uss2output`) and three non-empty files (`animal1`, `animal2`, `animal3`).
    -   **Looping & Variables:** The script utilizes `for` loops to iterate through file contents and variables like `$1` to accept user arguments (name).
-   **Permissions Management:**
    -   **Execution Rights:** The script was initially read-only. Used `chmod +x` to add the execution bit, allowing the shell to run the file as a program.
-   **I/O Redirection:**
    -   **Output Generation:** The script directs its output (standard out) into a log file named `message` using redirection operators (`>`), proving that the logic executed successfully.

---

## Technical Details

-   **Language:** UNIX Shell Scripting (Bash/Sh)
-   **Environment:** z/OS UNIX System Services (USS)
-   **Validation Job:** `ZXP.PUBLIC.JCL(CHKUSS2)`
-   **Key Commands:**
    -   `chmod +x animals.sh` (Change Mode)
    -   `mkdir uss2output` (Make Directory)
    -   `echo "lion" > animal1` (Input Creation)
    -   `./animals.sh Paarth` (Execution with Argument)

---

## Contact

For any questions or feedback, reach out:
**Paarth Pandey**
[LinkedIn](https://www.linkedin.com/in/paarth-pandey-13779529b/) | [GitHub](https://github.com/paarthpandey10) | paarthdxb@gmail.com

---

> Author: [Paarth Pandey](https://github.com/paarthpandey10)
>
> IBM Z Xplore - Advanced
