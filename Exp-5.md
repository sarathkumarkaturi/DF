# Experiment No. 5: Digital Forensic Investigation Using Autopsy

## Aim

To create a forensic case in Autopsy, add a forensic disk image as a data source, configure the ingest modules, and analyze the acquired forensic data.

---

## Software Used

- Autopsy 4.23.1
- Windows Operating System
- Forensic Disk Image (.E01)

---

## Introduction

Autopsy is an open-source digital forensics platform used to investigate digital evidence. It provides a graphical interface for examining disk images, files, web activity, operating system information, deleted files, and other digital artifacts.

In this experiment, Autopsy is used to create a new forensic case and add a forensic disk image for analysis.

---

# Procedure

## Step 1: Open Autopsy

Open the Autopsy application.

The Autopsy welcome screen provides options such as:

- New Case
- Open Recent Case
- Open Case

Select **New Case** to create a new forensic investigation case.

<img width="416" height="272" alt="1" src="https://github.com/user-attachments/assets/329c4b9e-032c-4fcb-b429-f4a613330a68" />


---

## Step 2: Create a New Case

Select **New Case** and enter the case information.

The following details were entered:

- **Case Name:** 05
- **Base Directory:** D:\3-1\Digital Forensics\EXP-5
- **Case Type:** Single-User

The case data will be stored in:

`D:\3-1\Digital Forensics\EXP-5\05`

Click **Next** to continue.

<img width="585" height="346" alt="2" src="https://github.com/user-attachments/assets/6aefc8bc-1ae5-4cfb-9bbd-de48e83eace9" />


---

## Step 3: Enter Optional Case Information

Enter the additional information about the case and examiner.

The following information was entered:

- **Case Number:** 05
- **Examiner Name:** Sarath
- **Phone:** 9059376605
- **Email:** 99240041243@klu.ac.in
- **Organization:** Not Specified

Click **Finish** to create the case.

<img width="586" height="343" alt="3" src="https://github.com/user-attachments/assets/b24d36af-e068-43d5-8dc5-a9201c6a454a" />


---

## Step 4: Create the Case

After clicking Finish, Autopsy starts creating the case and opening the required case-level services.

The application displays a progress window while the case is being created.

<img width="316" height="159" alt="4" src="https://github.com/user-attachments/assets/3c6f019b-9c7d-444e-9ed3-1580626f6808" />


---

## Step 5: Add a Data Source

After the case is created, select **Add Data Source**.

Autopsy provides different options for organizing the data source using hosts.

The default option selected is:

**Generate new host name based on data source name**

Click **Next** to continue.

<img width="315" height="203" alt="5" src="https://github.com/user-attachments/assets/dac24e99-cfbf-4e6d-a78e-a351d9f3592f" />


---

## Step 6: Select Data Source Type

Autopsy provides several data source types, including:

- Disk Image or VM File
- Local Disk
- Logical Files
- Unallocated Space Image File
- Autopsy Logical Imager Results
- XRY Text Export

For this experiment, the **Disk Image or VM File** option is used.

<img width="647" height="419" alt="6" src="https://github.com/user-attachments/assets/918b7494-f22d-455f-8aca-4ca3c753346b" />


---

## Step 7: Select the Forensic Disk Image

Select the forensic disk image that will be analyzed.

The selected image file is:

`C:\Users\sarath\Downloads\4Dell Latitude C\P (1).E01`

The time zone selected is:

**(GMT+5:30) Asia/Calcutta**

The sector size is set to:

**Auto Detect**

The BitLocker password and hash values are left empty because they were not provided.

Click **Next** to continue.

<img width="647" height="409" alt="7" src="https://github.com/user-attachments/assets/82ce41ed-906b-435f-b690-b80c4a42c095" />

---

## Step 8: Configure Ingest Modules

Autopsy provides several ingest modules for processing and analyzing the forensic data.

The screenshot shows multiple modules selected, including:

- Encryption Detection
- Interesting Files Identifier
- Central Repository
- PhotoRec Carver
- Virtual Machine Extractor
- Data Source Integrity
- Android Analyzer (aLEAPP)
- Cyber Triage Malware Scanner
- DJI Drone Analyzer
- Plaso
- YARA Analyzer
- iOS Analyzer (iLEAPP)
- GPX Parser
- Android Analyzer

These modules help Autopsy identify and extract useful forensic artifacts from the data source.

<img width="643" height="403" alt="8" src="https://github.com/user-attachments/assets/91def474-d555-4bea-8bb2-46dc00689ef8" />


---

## Step 9: Add and Process the Data Source

After configuring the ingest modules, Autopsy processes the selected forensic data source and adds it to the local case database.

The processing may take some time depending on the size of the forensic image.

<img width="646" height="402" alt="9" src="https://github.com/user-attachments/assets/13a29322-4ba4-4a27-96f8-8cbfce47f702" />


---

## Step 10: Analyze the Added Data Source

After the data source is added, Autopsy displays the forensic case interface.

The Directory Tree contains different categories for analyzing the evidence, including:

- Data Sources
- File Views
- File Types
- Deleted Files
- File Size
- Data Artifacts
- Metadata
- Operating System Information
- Recent Documents
- Run Programs
- Web Bookmarks
- Web Cookies
- Web History
- Analysis Results
- Encryption Suspected
- Extension Mismatch Detected
- Interesting Items
- Web Categories
- OS Accounts
- Tags
- Score
- Reports

The data source is displayed under the **Data Sources** section.

<img width="641" height="404" alt="10" src="https://github.com/user-attachments/assets/46d27b91-cee1-4b83-985b-ee09c9ff1441" />


---

## Step 11: Observe the Analysis Progress

Autopsy continues analyzing the files from the forensic disk image.

The analysis progress is displayed at the bottom of the Autopsy window.

The forensic image is shown as the added data source, and the analysis results are available through the Directory Tree.

<img width="861" height="580" alt="11" src="https://github.com/user-attachments/assets/0015eeca-f4dc-480d-b584-074baf79a6de" />


# Observations

The following observations were made during the experiment:

1. A new forensic case named **05** was created.
2. The case was configured as a **Single-User** case.
3. Examiner information was added to the case.
4. A forensic disk image with the `.E01` extension was selected as the data source.
5. The time zone was set to **GMT+5:30 Asia/Calcutta**.
6. The sector size was set to **Auto Detect**.
7. Multiple Autopsy ingest modules were enabled for forensic analysis.
8. The forensic image was processed and added to the local case database.
9. Autopsy displayed different categories of forensic artifacts and analysis results.
10. The forensic image was successfully loaded for further investigation.

---

# Result

A forensic case was successfully created in Autopsy. The forensic `.E01` disk image was added as a data source and processed using the selected ingest modules.

The forensic data was successfully loaded into Autopsy and made available for further analysis through the Directory Tree and Analysis Results sections.

---

# Conclusion

The experiment demonstrated the basic process of digital forensic investigation using Autopsy. A forensic case was created, a disk image was added, ingest modules were configured, and the evidence was processed for analysis.

Autopsy provides a structured environment for examining digital evidence and identifying useful forensic artifacts from a disk image.
