# Visual Guide – ASM1: Introduction to Assembler

> A step-by-step visual walkthrough of compiling, linking, and executing Assembler code on z/OS.

---

## Step-by-Step Screenshots

### ✅ Step 1: Source Code Setup
*Preparing the environment. I navigated to the public directory `/z/public/assembler/` to locate the source file `fibonacci.s`. [cite_start]I then copied this file into my own working directory using `cp fibonacci.s /z/z87191/assembly/fibonacci.s` to ensure I had a local copy to work with[cite: 198, 200].*
![Step 1](./screenshots/01.png)

### ✅ Step 2: Build and Execute
*The compilation pipeline. This screenshot captures the three critical phases of the build process:*
1.  [cite_start]**Assemble:** Ran `as -o fibonacci.o fibonacci.s` to compile the source code into a binary object file[cite: 206].
2.  [cite_start]**Link:** Executed `ld -o fibonacci fibonacci.o` to link the object file with system libraries, creating the executable[cite: 210].
3.  **Run:** Triggered the program with `./fibonacci`. [cite_start]The terminal successfully output the first 38 numbers of the Fibonacci sequence (ending in `39088169`), confirming the logic was correct[cite: 214, 228].
![Step 2](./screenshots/02.png)

### ✅ Step 3: Final Validation
*Claiming the points. [cite_start]I submitted the validation JCL using `tsocmd submit "'ZXP.PUBLIC.JCL(CHKASM1)'"`[cite: 238]. The screenshot shows the job submission confirmation in the terminal and the corresponding Job `JOB07963` in Zowe Explorer returning with **CC 0000**, verifying the challenge was complete.*
![Step 3](./screenshots/03.png)

---

## What I Learned

-   [cite_start]**The "Build" Pipeline:** How programs go from Source Code (`.s`) $\to$ Object File (`.o`) $\to$ Executable Binary[cite: 207, 211].
-   [cite_start]**Direct Memory Access:** Unlike high-level languages, Assembler requires managing specific registers and memory addresses directly to perform calculations[cite: 44, 46].
-   [cite_start]**System Calls:** How to use service programs like `BPX1WRT` to perform standard operations (like printing to stdout) since the Assembler language does not have a direct instruction for displaying values[cite: 192].
-   [cite_start]**Looping Logic:** Using the `BCT` (Branch on Count) instruction to iterate through the calculation 38 times[cite: 153].

---

## Notes

-   **Source File:** `fibonacci.s`
-   **Executable:** `fibonacci`
-   [cite_start]**Key OpCodes:** `BCT` (Loop), `MVC` (Move Character), `BAS` (Branch and Save)[cite: 148, 153, 161].

---

## Contact

**Paarth Pandey**
[LinkedIn](https://www.linkedin.com/in/paarth-pandey-13779529b/) | [GitHub](https://github.com/paarthpandey10) | paarthdxb@gmail.com

---

## Credits

This lab is based on the [IBM Z Xplore Learning Platform](https://ibmzxplore.influitive.com/), provided by IBM.
Visuals, objectives, and task flows belong to IBM and are used under fair use for personal learning documentation.

—

> Author: [Paarth Pandey](https://github.com/paarthpandey10)
>
> IBM Z Xplore: Advanced
