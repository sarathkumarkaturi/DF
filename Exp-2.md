# Digital Forensics – TestDisk Data Recovery

## Experiment No. 2

### Recover Deleted or Damaged Files from a Storage Device Using TestDisk

---

## Aim

To recover deleted or damaged partitions/files from a storage device using **TestDisk** and to analyze and repair partition and filesystem-related problems.

---

## Objective

- To understand the working of TestDisk.
- To identify the partition structure of a storage device.
- To search for lost or deleted partitions.
- To verify the files present in a recovered partition.
- To recover a lost partition by updating the partition structure.
- To identify and repair a damaged NTFS boot sector.

---

## Software Used

- **TestDisk 7.3-WIP**
- Windows operating system
- Computer internal SSD

---

## Introduction

TestDisk is a free and open-source data recovery utility used to recover lost partitions and make non-booting disks bootable again.

It can also be used to repair certain filesystem problems and recover data from damaged or deleted partitions.

In this experiment, TestDisk was used to analyze the partition structure of a storage device, search for partitions, identify filesystem problems, and proceed with partition recovery.

---

## Procedure

### Step 1 – Create TestDisk Log

Start TestDisk with administrator privileges.

TestDisk displays three options:

- Create – Create a new log file
- Append – Append information to an existing log
- No Log – Do not create a log

The **Create** option was selected to record the technical information and operations performed during the recovery process.

<img width="1960" height="1082" alt="1" src="https://github.com/user-attachments/assets/76b29ee9-fdc5-4d21-b7ca-22cd0e7671e1" />


---

### Step 2 – Select the Storage Device

TestDisk displays the available storage devices.

The detected storage device was:

- PhysicalDrive0
- Capacity: 250 GB / 232 GiB
- Model: CT250P2SSD8

The required disk was selected and **Proceed** was chosen.

<img width="1974" height="1086" alt="2" src="https://github.com/user-attachments/assets/afec6cc0-3a69-4be6-a863-8e32744e5777" />

---

### Step 3 – Select Partition Table Type

TestDisk displayed different partition table types such as:

- Intel/PC
- EFI GPT
- Humax
- Mac
- None
- Sun
- Xbox

TestDisk automatically detected the partition table as **EFI GPT**.

The detected **EFI GPT** option was selected and Enter was pressed.

<img width="1840" height="1000" alt="3" src="https://github.com/user-attachments/assets/ade14945-96f7-4209-a725-5948e414d4d4" />


---

### Step 4 – Analyse the Partition Structure

TestDisk displayed the available options:

- Analyse
- Advanced
- Geometry
- Options
- MBR Code
- Delete
- Quit

The **Analyse** option was selected to examine the current partition structure and search for lost partitions.
<img width="1946" height="1054" alt="4" src="https://github.com/user-attachments/assets/b0b2ce05-e402-4534-a970-540a80304f40" />


---

### Step 5 – Examine Current Partition Structure

TestDisk displayed the current partition structure of the selected disk.

The partition information was analyzed to identify missing partitions and filesystem errors.

The **Quick Search** option was selected to search for lost partitions.

<img width="1990" height="1086" alt="5" src="https://github.com/user-attachments/assets/831f04b8-d742-4e2c-a43b-cb88d51ae02d" />


---

### Step 6 – Quick Search and Filesystem Warning

During the search, TestDisk displayed information about the detected partitions.

A warning was displayed indicating that the detected disk size appeared inconsistent with the partition information.

The NTFS partition information was also displayed.

This indicates that TestDisk was examining the partition structure and filesystem information for possible recovery.

<img width="1910" height="1042" alt="6" src="https://github.com/user-attachments/assets/401c5e0e-5bb3-4230-86c5-9b7d37cfe4b3" />


---

### Step 7 – Identify Detected Partitions

TestDisk displayed the partitions found during the search.

The detected partition entries included:

- FAT32 – EFI System Partition
- HPFS - NTFS partitions

The partition structure was examined to determine the valid partitions.

TestDisk allows the user to change the status of a detected partition using the left/right arrow keys.

Possible partition statuses include:

- Primary
- Bootable
- Logical
- Deleted

A partition marked as deleted can be changed to the appropriate partition type when it is confirmed to be the correct partition.

<img width="1962" height="1076" alt="7" src="https://github.com/user-attachments/assets/08731a53-41b3-4b9a-9402-6e3b4e08bc72" />


---

### Step 8 – Complete the Operation and Restart

After the partition recovery operation, TestDisk displayed a message indicating that the computer needed to be restarted for the changes to take effect.

The **OK** option was selected and the system was prepared for restart.

<img width="1962" height="1068" alt="8" src="https://github.com/user-attachments/assets/7fcbe593-ad4f-40ad-b099-d7b368344576" />


---

## Working Principle

The basic working process of TestDisk in this experiment was:

```text
Start TestDisk
       ↓
Create Log
       ↓
Select Storage Device
       ↓
Detect Partition Table
       ↓
Analyse Partition Structure
       ↓
Quick Search
       ↓
Identify Lost/Damaged Partitions
       ↓
Verify Partition Information
       ↓
Recover/Update Partition Structure
       ↓
Restart System
