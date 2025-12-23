# USS1 – UNIX System Services Screenshots

> Visual reference for SSH connections, command-line navigation, and script execution steps performed during the USS1 challenge.

---

## Overview

This folder contains screenshots verifying the successful completion of the USS1 lab.
The images document the workflow of connecting to the z/OS UNIX environment, executing the `scramble.sh` challenge, and correctly redirecting output for validation.

---

## Image Manifest

- **01.png:** Establishing the SSH connection to the mainframe IP (`204.90.115.200`).
- **02.png:** Running `uss-setup` to populate the home directory with challenge files.
- **03.png:** Using `ls -l` to inspect permissions and identify the executable `scramble.sh`.
- **04.png:** executing `./scramble.sh` with the correct rotation argument to reveal the secret message.
- **05.png:** Redirecting the decoded output to `ussout.txt` using the `>` operator.
- **06.png:** Appending disk usage (`du -ak`) and timestamp (`date`) to the output file using `>>`.
- **07.jpg:** Viewing the final `ussout.txt` file inside the Zowe Explorer USS view.

---

## Contact

For any questions or feedback, reach out:
**Paarth Pandey**
[LinkedIn](https://www.linkedin.com/in/paarth-pandey-13779529b/) | [GitHub](https://github.com/paarthpandey10) | paarthdxb@gmail.com

---

> Author: [Paarth Pandey](https://github.com/paarthpandey10)
>
> IBM Z Xplore - Fundamentals