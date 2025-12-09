# [VSC1: Connect to Z]

> Setting up the modern mainframe development environment using VS Code and Zowe Explorer.

---

## Overview

This module documents the initial setup and configuration required to connect to the IBM Z Xplore mainframe environment. The objective was to move away from traditional "green screen" emulators and establish a modern workflow using **VS Code** and the **Zowe Explorer** extension.

This setup bridges the gap between modern DevOps tooling and legacy mainframe infrastructure, allowing for easier dataset management and job submission.

---

## Key Highlights

- **Environment Configuration:** Installed Node.js and the IBM Z Open Editor extension to enable mainframe language support (COBOL, JCL, REXX).
- **Zowe Profile Setup:** Configured a Zowe Team Configuration (`zowe.config.json`) to connect to the IBM Z host at `204.90.115.200` on port `10443`.
- **Security Bypass:** Configured the profile to handle self-signed certificates by setting `rejectUnauthorized: false` for the lab environment.
- **Connection Validation:** Successfully filtered datasets using my Z-ID and submitted the validation job `CHKVSC` located in `ZXP.PUBLIC.JCL` to confirm system access.

---

## Technical Details

- **Host IP:** `204.90.115.200`
- **Port:** `10443` (z/OSMF)
- **Validation Job:** `ZXP.PUBLIC.JCL(CHKVSC)`
- **Tools:** Zowe Explorer, IBM Z Open Editor

---

## Contact

For any questions or feedback, reach out:
**Paarth Pandey** [LinkedIn](https://www.linkedin.com/in/paarth-pandey-13779529b/) | [GitHub](https://github.com/paarthpandey10) | paarthdxb@gmail.com

---

> Author: [Paarth Pandey](https://github.com/paarthpandey10)
>
> IBM Z Xplore - Fundamentals
