# Experiment No. 6: Use Sleuth Kit to Analyze Digital Evidence

## Aim

To use the Sleuth Kit command-line tools to analyze a forensic disk image, identify the file system and partitions, list files and directories, recover a file, and analyze file metadata.

## Software Used

- Sleuth Kit 4.14.0
- Windows PowerShell
- Forensic Disk Image

## Description

The Sleuth Kit (TSK) is a collection of command-line tools used for analyzing disk images and recovering digital evidence. In this experiment, the forensic disk image `4Dell Latitude CPi.E01` is analyzed using Sleuth Kit tools.

## Step 1: Install and Open Sleuth Kit

The Sleuth Kit tools were downloaded and the bin directory was opened. The bin directory contains tools such as fsstat.exe, mmls.exe, fls.exe, icat.exe, istat.exe and img_stat.exe.

<img width="959" height="599" alt="1" src="https://github.com/user-attachments/assets/90802aef-c97f-4096-b75b-f33ccff3c9d3" />


## Step 2: Identify the File System Using fsstat

The fsstat command was used to identify and analyze the file system present in the forensic image.

The output shows that the file system is NTFS and the image contains Windows XP file-system information.

<img width="479" height="398" alt="2" src="https://github.com/user-attachments/assets/ade35b64-ebb5-4312-9b58-fe7d71ff5f34" />


## Step 3: List Partitions Using mmls

The mmls command was used to identify the partition structure of the forensic disk image.

The output shows the DOS partition table and an NTFS/exFAT partition.

<img width="489" height="287" alt="3" src="https://github.com/user-attachments/assets/a86de16d-1f6f-48dd-9b32-5b5a9bc008a9" />


## Step 4: Analyze Files and Directories Using fls

The fls command was used to recursively list the files and directories contained in the forensic image.

The output was saved into file_list.txt.

<img width="475" height="403" alt="4" src="https://github.com/user-attachments/assets/de36c3a2-1af5-4d51-8ef3-9f8b6ca4b11c" />


## Step 5: Recover a File Using icat

The inode number of excel.xls was identified from the file listing. The icat command was then used to recover the file from the forensic image.

The recovered file was saved as: recovered_excel.xls

<img width="480" height="599" alt="6" src="https://github.com/user-attachments/assets/d91220fc-1477-4204-94bc-258ac0f0becd" />


## Step 6: Analyze File Metadata Using istat

The istat command was used to analyze the metadata associated with the excel.xls file.

<img width="463" height="102" alt="7" src="https://github.com/user-attachments/assets/8d16bd92-5300-4dc9-9767-bd312f032245" />


## Step 7: Examine the Generated File List

The generated file_list.txt file was opened to examine the files and directories identified by Sleuth Kit.

<img width="463" height="99" alt="5" src="https://github.com/user-attachments/assets/918ba1a6-cd25-457e-9e2f-853e25a22b3a" />


## Step 8: Timeline Analysis (Optional)

The experiment manual specifies timeline analysis as an optional step. A body file was generated using fls.

The Sleuth Kit Windows package contains mactime.pl rather than mactime.exe. Perl was not available in the Windows environment, so the optional mactime timeline generation was not executed.

<img width="461" height="235" alt="9" src="https://github.com/user-attachments/assets/f1049b15-8dd2-40b7-9e01-2895d1d40702" />


## Step 9: Generate and Collect the Report Data

The generated analysis files were collected.

<img width="338" height="227" alt="10" src="https://github.com/user-attachments/assets/504cb8b9-60dd-4376-ad6f-1338038c37bb" />


## Result

The forensic disk image 4Dell Latitude CPi.E01 was successfully analyzed using Sleuth Kit.

The following operations were successfully performed:

- Identified the file system as NTFS using fsstat.
- Identified the partition structure using mmls.
- Listed files and directories using fls.
- Identified the inode of excel.xls.
- Recovered excel.xls using icat.
- Analyzed file metadata using istat.
- Generated a body file for optional timeline analysis.

The recovered file was saved as: recovered_excel.xls

## Conclusion

Sleuth Kit was successfully used to analyze the forensic disk image and extract digital evidence. The experiment demonstrated file-system analysis, partition identification, file listing, file recovery, and metadata analysis using command-line forensic tools.
