# Experiment No. 2: Recover Deleted or Damaged Files Using TestDisk

## Aim

To recover a deleted or missing partition and restore access to the files using TestDisk.

## Software Used

- TestDisk 7.3-WIP
- Windows Operating System
- USB Pendrive
- NTFS File System

## Introduction

TestDisk is a free and open-source data recovery utility used to recover lost partitions, repair damaged partition structures, and restore access to files from storage devices.

In this experiment, a 4 GB partition named `Testing` was created on a USB pendrive. The partition was deleted to simulate data loss. TestDisk was then used to analyse the USB pendrive, locate the deleted partition, verify the files stored in it, and restore the partition structure.

## Procedure

### Step 1: Open TestDisk

Open `testdisk_win.exe` with administrator privileges.

TestDisk displays information about the data recovery utility and provides options for creating or appending a log file.

Select:

`Create`

and press **Enter** to create a new log file.

<img width="439" height="292" alt="1" src="https://github.com/user-attachments/assets/7b26fc92-1680-4b73-8985-a4d8238281af" />


**Observation:** TestDisk was successfully started and the option to create a new log file was selected.

---

### Step 2: Select the USB Pendrive

TestDisk displays all detected physical storage devices.

The USB pendrive was identified as:

- PhysicalDrive1
- 125 GB / 117 GiB
- USB DISK 2.0

Select the USB pendrive and choose:

`Proceed`

<img width="479" height="305" alt="2" src="https://github.com/user-attachments/assets/71e5841f-0899-4fd9-a827-50f37406c205" />


**Observation:** The 117 GB USB pendrive was correctly identified and selected for the recovery process.

---

### Step 3: Analyse the Disk

After selecting the USB pendrive, TestDisk displays the main menu.

The available options include:

- Analyse
- Advanced
- Geometry
- Options
- MBR Code
- Delete
- Quit

Select:

`Analyse`

to analyse the current partition structure and search for lost partitions.

<img width="482" height="308" alt="3" src="https://github.com/user-attachments/assets/d46d4ba4-870d-46c5-93d3-c0197ce367ab" />


**Observation:** The Analyse option was selected to search for the deleted partition.

---

### Step 4: Perform Quick Search

TestDisk displays the current partition structure of the USB pendrive.

The existing `SARATH'S` partition is displayed.

Select:

`Quick Search`

and press **Enter**.

<img width="485" height="316" alt="4" src="https://github.com/user-attachments/assets/c240dca3-acde-4b80-b4bb-964c650d492d" />


**Observation:** TestDisk started searching for lost or deleted partitions.

---

### Step 5: Verify the Deleted Partition

TestDisk detects the deleted `Testing` partition.

Select the `Testing` partition and press:

`P`

The `P` option is used to list the files stored in the selected partition.

<img width="479" height="311" alt="5" src="https://github.com/user-attachments/assets/4d9ebd74-db10-4cf6-90d2-54ac61c9ea53" />


**Observation:** TestDisk successfully displayed the files from the deleted `Testing` partition. The displayed files included images and screenshots that were previously stored in the partition.

Examples of detected files include:

- `1.jpg`
- `2345.jpg`
- `Screenshot 2026-09-07 203856.png`
- `WIN_20250914_21_21_06_Pro.jpg`
- `WIN_20251207_20_53_37_Pro.jpg`
- `WIN_20251208_13_29_03_Pro.jpg`

This confirms that the deleted partition and its file system data were successfully detected.

Press `q` to return to the partition list.

---

### Step 6: Confirm the Recovered Partition

After returning to the partition list, TestDisk displays both the deleted `Testing` partition and the existing `SARATH'S` partition.

The detected partition structure is:

- `Testing` – approximately 4 GB
- `SARATH'S` – approximately 113 GB

The screen displays:

`Structure: Ok.`

<img width="484" height="311" alt="6" src="https://github.com/user-attachments/assets/6a345702-3737-49c4-ba53-48433df65ada" />


**Observation:** The deleted `Testing` partition was successfully detected and the partition structure was reported as OK.

Press **Enter** to continue.

---

### Step 7: Write the Recovered Partition Structure

TestDisk provides the:

`Write`

option to save the detected partition structure to the USB pendrive.

<img width="482" height="308" alt="7" src="https://github.com/user-attachments/assets/d8767109-5811-4536-81c9-c549f3217091" />


Select:

`Write`

and press **Enter**.

Confirm the operation when TestDisk asks for confirmation.

**Observation:** The recovered partition structure was selected to be written back to the USB pendrive.

---

## Result

The deleted 4 GB `Testing` partition was successfully detected using TestDisk. The files stored in the deleted partition were successfully displayed using the `P` option, confirming that the partition data was recoverable.

The recovered partition structure was then selected using the `Write` option.

## Conclusion

The experiment successfully demonstrated the recovery of a deleted partition using TestDisk. The USB pendrive was analysed, the deleted `Testing` partition was located using Quick Search, the files were verified using the `P` option, and the recovered partition structure was selected for writing back to the storage device.

