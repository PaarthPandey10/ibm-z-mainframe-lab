# Visual Guide – USS1: UNIX System Services

> A step-by-step visual walkthrough of using the UNIX shell on IBM Z to solve the scramble challenge.

---

## Step-by-Step Screenshots

### ✅ Step 1: Connect via SSH
*Opening the PowerShell terminal on Windows and connecting to the z/OS system using the SSH protocol. I confirmed the host authenticity and logged in as user `z87191`.*
![Step 1](./screenshots/01.png)

### ✅ Step 2: Navigation & File Creation
*Exploring the directory structure. I navigated into the `test` directory to read the `hello-there` file, then returned to the home directory to create a new empty file using `touch mynewfile`.*
![Step 2](./screenshots/02.png)

### ✅ Step 3: The Scramble Challenge (Trial & Error)
*Running the decryption script. I initially tried a rotation key of **12**, which resulted in gibberish (`xjibmv...`). After further deduction, I found the correct rotation key was **17**, which successfully revealed the message: "congratulations! you unscrambled the message..."*
![Step 3](./screenshots/03.png)

### ✅ Step 4: Redirection & Appending
*Once the key (17) was confirmed, I used output redirection (`>`) to save the decoded message to `ussout.txt`. I then used the append operator (`>>`) to add the current system `date` to the bottom of the file.*
![Step 4](./screenshots/04.png)

### ✅ Step 5: Final Validation
*Checking the Zowe Explorer "JOBS" view to verify the submission. The validation job `chkuss1(JOB07233)` completed with **CC 0000**, confirming the challenge was passed successfully.*
![Step 5](./screenshots/05.png)

---

## What I Learned

- **SSH (Secure Shell):** How to remotely access the z/OS UNIX command line interface from a Windows PowerShell environment.
- **Trial & Error:** Using standard shell execution (`./scramble.sh`) to test different arguments (rotation keys 12 and 17) until the logic held up.
- **I/O Redirection:** The power of `>` to create files from output and `>>` to append log data like timestamps.
- **Zowe Integration:** Using the Zowe Explorer to instantly verify JCL job completion codes (`CC 0000`) without leaving VS Code.

---

## Notes

- **Identity:** Logged in as `z87191` on IP `204.90.115.200`.
- **Command History:** Utilized `cd`, `ls`, `cat`, `touch`, and `./` execution throughout the lab.

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
> IBM Z Xplore: Fundamentals