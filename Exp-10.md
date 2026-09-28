# Experiment-10 Use Ghidra to Disassemble and Analyze a Binary

## Aim

To use **Ghidra** to load, disassemble, analyze, and examine a binary file by creating a project, importing the binary, performing automatic analysis, and studying the program structure and assembly code.

---

## Requirements

- Ghidra
- Java Runtime Environment
- Windows / Linux / macOS
- Sample binary file
- Computer system

---

## Step 1: Open Ghidra

Launch **Ghidra** on the system.

The Ghidra startup window is displayed successfully.

The Ghidra version and Java version are shown on the startup screen.

<img width="414" height="237" alt="10 (1)" src="https://github.com/user-attachments/assets/2ed66237-e1b2-4099-8715-a765f873bd6c" />

---

## Step 2: Create a New Project

Open Ghidra and select:

**File → New Project**

The New Project option is selected from the Ghidra File menu.

<img width="451" height="296" alt="10 (2)" src="https://github.com/user-attachments/assets/d569bff5-cffd-4839-a465-f7fd1c1133c4" />

---

## Step 3: Select Project Type

In the **Select Project Type** window, select:

**Non-Shared Project**

Click **Next** to continue creating the project.

<img width="449" height="245" alt="10 (3)" src="https://github.com/user-attachments/assets/5e0ddb8d-9934-44ad-87b2-4462d7a7c810" />

---

## Step 4: Open the Ghidra Project

The Ghidra project is created and opened successfully.

The project name used for the experiment is:

```text
hackverse_ctf
```

The project workspace is displayed in Ghidra.

<img width="444" height="271" alt="10 (4)" src="https://github.com/user-attachments/assets/706f10ce-f5f9-4e10-956f-991072751650" />

---

## Step 5: Import the Binary File

From the Ghidra project window, select:

**File → Import File**

The Import File option is selected from the File menu to add the binary to the project.

<img width="451" height="231" alt="10 (5)" src="https://github.com/user-attachments/assets/3d72d004-5446-4a0f-a843-7227e09ac3cb" />

---

## Step 6: Select the Binary File

Select the required binary file from the system.

The binary file used in this experiment is:

```text
binary1 (1)
```

The selected binary file is opened for importing into the Ghidra project.

<img width="459" height="293" alt="10 (6)" src="https://github.com/user-attachments/assets/f73a9b66-9904-4895-ac43-e2856621cd7b" />

---

## Step 7: Configure the Binary Import

Ghidra automatically detects the binary file format.

The import window displays the following information:

```text
Format:
Executable and Linking Format (ELF)

Language:
x86:LE:64:default:gcc

Destination Folder:
hackverse_ctf/

Program Name:
binary1 (1)
```

Click **OK** to import the binary.

<img width="363" height="288" alt="10 (7)" src="https://github.com/user-attachments/assets/537a7352-990e-4dea-8ce3-efa39ac93c94" />

---

## Step 8: View the Import Results

After importing the binary, Ghidra displays the **Import Results Summary**.

The summary contains information about:

- Project File Name
- Program Name
- Language ID
- Compiler ID
- Processor
- Endian
- Address Size
- Minimum Address
- Maximum Address
- Number of Bytes
- Number of Memory Blocks
- Number of Instructions
- Number of Defined Data
- Number of Functions
- Number of Symbols
- Number of Data Types
- Ghidra Version

The binary is successfully imported into the Ghidra project.

<img width="357" height="140" alt="10 (8)" src="https://github.com/user-attachments/assets/1a826518-6f67-43f0-b473-737ec33c16f0" />

---

## Step 9: Start Automatic Analysis

Open the imported binary in Ghidra.

Ghidra displays a message asking whether the binary should be analyzed.

Select:

**Yes**

The **Analysis Options** window is displayed.

The available analysis options are enabled and the analysis is started.

<img width="355" height="174" alt="10 (9)" src="https://github.com/user-attachments/assets/572e3091-3a4a-4aba-a8f7-4bbc5cd2c785" />

---

## Step 10: Analyze the Binary

After automatic analysis is completed, the binary is opened in the **CodeBrowser**.

The CodeBrowser displays:

- Program Tree
- Symbol Tree
- Data Type Manager
- Imports
- Exports
- Functions
- Labels
- Memory sections
- Assembly instructions
- Decompiler window

The assembly instructions and program functions can be examined to understand the structure and behavior of the binary.

<img width="360" height="183" alt="10 (10)" src="https://github.com/user-attachments/assets/79598f5b-7b98-4086-bd21-74b523970ef6" />

---

## Result

The binary file was successfully loaded, imported, and analyzed using **Ghidra**.

A Ghidra project was created, the ELF binary was imported, automatic analysis was performed, and the analyzed binary was opened in the CodeBrowser.

The program structure, functions, imports, labels, memory sections, and assembly instructions were successfully examined.

---
