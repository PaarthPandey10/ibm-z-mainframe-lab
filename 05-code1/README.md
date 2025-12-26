# CODE1: Python on IBM Z

> leveraging the Python programming language within the z/OS UNIX System Services environment.

---

## Overview

This module documents the **CODE1** challenge of the IBM Z Xplore series. While the previous challenge (USS1) introduced the UNIX shell, this challenge demonstrates the modernization of the mainframe by running **Python** workloads. The goal was to edit and execute Python scripts to manipulate strings, handle loops, and perform arithmetic operations directly on z/OS.

---

## Key Highlights

- **Python Execution:**
  - Executed Python scripts using the `python3` command directly in the z/OS UNIX shell.
  - Ran `code1.py` which interacted with system time and processed User ID integers.
- **Logic & Control Flow:**
  - Utilized `if/else` statements in `code2.py` to check for characters within string variables.
  - Created a `while` loop in `marbles.py` to count down inventory from 10 to 0.
- **String Manipulation:**
  - Implemented string slicing (e.g., `marble_dots[0:marbles]`) to create dynamic visual outputs based on variable state.
  - Used f-string style concatenation (e.g., `"You have " + str(marbles)`) to combine integers and text.
- **Validation:**
  - Submitted the `CHKCODE` job via Zowe Explorer to verify the script logic.

---

## Technical Details

- **Language:** Python 3
- **Validation Job:** `ZXP.PUBLIC.JCL(CHKCODE)`
- **Key Concepts:**
  - **Loops:** `while (marbles > 0):`
  - **Conditionals:** `if (marbles <= 3):`
  - **Slicing:** `string[start:end]`
  - **Integration:** Editing z/OS files using the standard VS Code editor interface.
- **Tools:** VS Code, Zowe Explorer, Python Interpreter.

---

## Contact

For any questions or feedback, reach out:
**Paarth Pandey**
[LinkedIn](https://www.linkedin.com/in/paarth-pandey-13779529b/) | [GitHub](https://github.com/paarthpandey10) | paarthdxb@gmail.com

---

> Author: [Paarth Pandey](https://github.com/paarthpandey10)
>
> IBM Z Xplore - Fundamentals
