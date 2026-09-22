# Experiment 9 – Process Explorer

## Aim

To use Process Explorer to examine running processes, analyze CPU and memory usage, inspect process properties, check network activity, and identify potentially suspicious processes.

## Software Required

- Windows Operating System
- Process Explorer (Sysinternals)
- Windows Security

## Procedure

### Step 1 – Download and Extract Process Explorer

Process Explorer was downloaded and extracted into the `ProcessExplorer` folder.

The folder contained:

- procexp.exe
- procexp64.exe
- procexp64a.exe
- Eula.txt

<img width="480" height="328" alt="1" src="https://github.com/user-attachments/assets/494ddab1-e764-4029-ab47-5919db87d033" />


---

### Step 2 – Run Process Explorer as Administrator

The `procexp64.exe` application was executed using **Run as administrator**.

Process Explorer displayed the running processes in a hierarchical process tree.

<img width="959" height="599" alt="2" src="https://github.com/user-attachments/assets/d69767a0-a182-4e14-8ad6-5c51f90b28f9" />


---

### Step 3 – Examine Running Processes

The Process Explorer window was examined using the following columns:

- Process
- CPU
- Private Bytes
- Working Set
- PID
- Description
- Company Name

The process tree was inspected to identify processes and their resource usage.




---

### Step 4 – Inspect Process Properties

The `svchost.exe` process was selected and its Properties window was opened.

The Image tab provided the following information:

- Process name: `svchost.exe`
- PID: `1944`
- Description: Host Process for Windows Services
- Path: `C:\Windows\System32\svchost.exe`
- User: `NT AUTHORITY\SYSTEM`
- Company: Microsoft Corporation

The executable path was inspected to verify that the process was running from the Windows System32 directory.

<img width="959" height="599" alt="3" src="https://github.com/user-attachments/assets/fad7549a-ff6c-4f12-8ba7-af541fa29743" />


---

### Step 5 – Inspect TCP/IP Activity

The TCP/IP tab of the `svchost.exe` Properties window was opened.

The Local Address, Remote Address, Protocol, State and Service information were inspected.

No TCP/IP connections were displayed for the selected process at the time of inspection.

<img width="472" height="109" alt="4" src="https://github.com/user-attachments/assets/181d3222-ac3d-40c8-bc3d-4b54a69aca36" />


---

### Step 6 – Examine CPU and Memory Usage

The CPU, Private Bytes and Working Set values were examined for the selected `svchost.exe` process.

Observed values included:

- CPU: `< 0.01`
- Private Bytes: `15,008 K`
- Working Set: `44,116 K`
- PID: `1944`

The process did not show unusually high CPU usage during the observation.



---

### Step 7 – Online Process Verification

The process name `svchost.exe` was searched online to understand its purpose.

The search results described `svchost.exe` as a Windows system process used to host and manage Windows services.



---

### Step 8 – Antivirus Check

Windows Security was opened and the Virus & threat protection section was examined.

<img width="1522" height="1033" alt="5" src="https://github.com/user-attachments/assets/3fb6ff7d-026c-41d8-ba55-aa4db152df0a" />



---

## Result

Process Explorer was successfully used to examine running Windows processes.

The `svchost.exe` process was investigated by checking its:

- Process ID
- CPU usage
- Memory usage
- Description
- Company name
- Executable path
- TCP/IP activity

The investigation showed that the selected `svchost.exe` process was located in the Windows System32 directory and was associated with Microsoft Corporation. No TCP/IP connections were displayed for the selected process during the inspection.

## Conclusion

Process Explorer provides detailed information about running Windows processes and their resource usage. It can be used in digital forensics and system investigation to examine process properties, identify unusual resource usage, inspect network activity, and investigate potentially suspicious processes.
