<img width="959" height="95" alt="Screenshot 2026-09-22 082017" src="https://github.com/user-attachments/assets/49243c16-ea7f-4d80-aba7-b9caeb01ec58" /># Experiment 7 – Use AFLogical OSE to Extract Data from an Android Device

## Aim

To use **AFLogical OSE (Open Source Edition)** to perform logical extraction of forensic data from an Android device and recover information such as **SMS messages and call logs**.

---

## Objective

The main objectives of this experiment are:

- To understand Android logical data extraction.
- To configure the Android Debug Bridge (ADB) environment.
- To connect an Android device to the computer.
- To install and use AFLogical OSE.
- To extract SMS messages from an Android device.
- To extract call log information from an Android device.
- To examine the extracted forensic data.

---

## Software and Requirements

- Windows Operating System
- Android smartphone
- AFLogical OSE
- Android Debug Bridge (ADB)
- Android Platform Tools
- Java Development Kit (JDK)
- USB cable
- USB Debugging enabled on the Android device
- Text editor for viewing extracted data

---

## Introduction

AFLogical OSE is an Android forensic data extraction tool developed for performing logical acquisition of information from Android devices.

It can be used to extract different types of user data, including:

- Call logs
- SMS messages
- Contacts
- MMS-related information

The extracted information can then be examined for digital forensic investigation.

---

# Procedure

## Step 1 – Prepare the AFLogical OSE Application

The AFLogical OSE application package was obtained and placed in a working folder on the computer.

The working folder contained the AFLogical application package required for installation on the Android device.

<img width="1233" height="695" alt="1" src="https://github.com/user-attachments/assets/e9511ef8-b123-42a5-b154-b0afffc66ba2" />


---

## Step 2 – Verify Java Installation

Java was installed and verified on the computer.

The installed Java environment was successfully detected and was ready for use with the Android forensic tools.

<img width="959" height="127" alt="Screenshot 2026-09-22 082011" src="https://github.com/user-attachments/assets/225bdfab-5926-4ac5-9b6a-00a367158719" />


## Step 3 – Verify Android Debug Bridge

Android Platform Tools were configured on the computer.

ADB was successfully detected and the Android Debug Bridge environment was ready for communication with the Android device.




---

## Step 4 – Connect the Android Device

The Android device was connected to the computer using a USB cable.

USB Debugging was enabled on the Android device.

The device was successfully detected by ADB.

The connected device was displayed in the list of available Android devices.

<img width="1076" height="235" alt="4" src="https://github.com/user-attachments/assets/53e0bebc-2d58-4291-9696-f04e10691c68" />


---

## Step 5 – Install AFLogical OSE

The AFLogical OSE application was installed on the connected Android device.

The installation completed successfully, confirming that the application was successfully transferred and installed on the device.

<img width="1190" height="207" alt="5" src="https://github.com/user-attachments/assets/2ebc67cb-5a5d-4fee-99a8-e74ffef819a3" />



---

## Step 6 – Extract Android Forensic Data

After installation, the AFLogical OSE application was used to obtain logical forensic information from the Android device.

The extracted data included:

- SMS messages
- Call logs

The extracted information was saved as text files on the computer for further examination.



<img width="959" height="95" alt="Screenshot 2026-09-22 082017" src="https://github.com/user-attachments/assets/81a11988-030c-428e-aaca-3ee2235d9e2b" />


---

## Step 7 – Examine Call Log Data

The extracted call log information was opened and examined.

The recovered data contained information associated with phone calls, including details such as:

- Phone numbers
- Call duration
- Call date and time
- Call type
- Contact information
- Other available call-related metadata

### Screenshot 7 – Extracted Call Logs

<img width="1747" height="132" alt="7" src="https://github.com/user-attachments/assets/ea4f758d-1d2e-4ca3-943d-8ff20639d309" />


---

## Step 8 – Examine SMS Data

The extracted SMS information was opened and examined.

The recovered SMS records contained information such as:

- Sender or recipient address
- Message content
- Date and time
- Message identifiers
- Message status
- Service information

### Screenshot 8 – Extracted SMS Data

<img width="1907" height="985" alt="8" src="https://github.com/user-attachments/assets/c6206733-3fd6-40cf-95d7-3c29c919b4e7" />


---

## Step 9 – Detailed Examination of Extracted Data

The extracted forensic records were further examined to understand the available information.

The SMS records contained detailed metadata and message contents. This demonstrated that logical acquisition can recover useful information from an Android device for forensic examination.

### Screenshot 9 – Detailed SMS Records

<img width="1910" height="1078" alt="9" src="https://github.com/user-attachments/assets/46d4750a-768a-4cb3-9b55-3ec11e2586c5" />


---

# Observations


1. Java was successfully installed and detected.
2. Android Platform Tools were successfully configured.
3. ADB successfully detected the connected Android device.
4. AFLogical OSE was successfully installed on the device.
5. Logical forensic data was successfully extracted.
6. Call log information was recovered.
7. SMS information was recovered.
8. The extracted information contained useful metadata for forensic analysis.

---

# Extracted Data

The experiment successfully recovered the following categories of information:

| Data Type | Status |
|---|---|
| Android Device Detection | Successful |
| AFLogical OSE Installation | Successful |
| Call Logs | Extracted |
| SMS Messages | Extracted |
| SMS Metadata | Extracted |
| Call Metadata | Extracted |

---

# Forensic Significance

Logical extraction is useful in digital forensics because it allows investigators to obtain accessible user-level information from an Android device.

The recovered call logs and SMS messages can provide useful evidence during investigations.

The extracted information can help investigators understand:

- Communication history
- Contact with other phone numbers
- Message contents
- Communication timestamps
- Call duration
- Other available metadata

---

# Result

AFLogical OSE was successfully used to perform logical extraction from an Android device.

The experiment successfully recovered **call logs and SMS messages**, which were examined as part of the forensic analysis.

---

# Conclusion

This experiment demonstrated the use of **AFLogical OSE** for Android logical forensic extraction.

The Android device was successfully connected to the computer, AFLogical OSE was installed, and forensic information including **SMS messages and call logs** was successfully extracted and examined.

The experiment provided practical knowledge of Android device acquisition and the examination of extracted mobile forensic data.

---
