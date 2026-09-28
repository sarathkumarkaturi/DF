# Ex. No. 10 — Use Ghidra to Disassemble and Analyze Malware Code

## Digital Forensics Lab

### Aim / Description

**Ghidra** is a software reverse-engineering framework used to disassemble and analyze binary programs.

This experiment demonstrates how to create a Ghidra project, import a binary file, perform automatic analysis, and examine the disassembled program using the CodeBrowser.

> **Safety Note:** Use only benign or controlled sample binaries for this laboratory exercise. Do not execute unknown malware on a normal personal computer.

---

# Requirements

The following are required:

- Ghidra
- Java
- Windows / Linux / macOS system
- Sample binary file
- Isolated virtual machine (recommended)

---

# 1. Open Ghidra

Launch Ghidra and wait for the Ghidra main window to load.

The Ghidra interface provides options for creating projects, opening existing projects, importing files, and managing analysis.

### Screenshot 1

![Ghidra Startup](screenshots/exp10_01.png)

---

# 2. Create a New Project

From the Ghidra main window:

1. Select **File**.
2. Click **New Project**.
3. The project creation window will appear.
4. Select the required project type.

### Screenshot 2

![New Project Menu](screenshots/exp10_02.png)

---

# 3. Select Project Type

Ghidra provides different project types.

For this experiment, **Non-Shared Project** is selected.

Steps:

1. Select **Non-Shared Project**.
2. Click **Next**.
3. Continue with the project creation process.

### Screenshot 3

![Project Type](screenshots/exp10_03.png)

---

# 4. Import the Binary File

After creating the project, the binary file is imported into Ghidra.

From the project window:

1. Select **File**.
2. Select **Import File**.
3. Choose the binary file that needs to be analyzed.

### Screenshot 4

![Import File Menu](screenshots/exp10_04.png)

---

# 5. Select the Binary File

The file selection window is displayed.

Select the required binary file from the location where it is stored.

In this experiment, the selected file is:

```text
binary1 (1)
