# Experiment 1: Evidence Acquisition Using AccessData FTK Imager

## Aim

To acquire a forensic disk image from a physical storage device using AccessData FTK Imager and verify the integrity of the acquired image using MD5 and SHA1 hash values.

## Software Used

- AccessData FTK Imager 4.7.1.2
- Windows

## Introduction

FTK Imager is a computer forensic tool developed by AccessData. It is used for acquiring and analyzing digital forensic evidence.

FTK Imager can acquire:

- Volatile memory (RAM)
- Non-volatile memory such as hard disks and USB drives
- Physical drives
- Logical drives
- Image files
- Contents of folders
- CDs/DVDs

In this experiment, a physical USB storage device was acquired and converted into a forensic disk image.

## Procedure

### Step 1: Open FTK Imager

Open **AccessData FTK Imager 4.7.1.2**.

Navigate to the option for creating a disk image.

![Open FTK Imager](screenshots/1.png)

### Step 2: Select Evidence Source

Select **Physical Drive** and click **Next**.

![Select Source](screenshots/2.png)

### Step 3: Select Physical Drive

Select the physical drive that needs to be acquired.

The device used in this experiment was:

**SanDisk Cruzer Blade USB Device**

Click **Finish**.

![Select Drive](screenshots/3.png)

### Step 4: Select Image Type

Select **Raw (dd)** and click **Next**.

![Select Image Type](screenshots/4.png)

### Step 5: Enter Evidence Information

The following evidence information was entered:

- Case Number: 1
- Evidence Number: 1
- Unique Description: DF
- Examiner: SARATH KATURI
- Notes: EXP 1

Click **Next**.

![Evidence Information](screenshots/5.png)

### Step 6: Select Image Destination

The image was saved in the following destination:

`D:\3-1\Digital Forensics`

Image Filename:

`diskimage`

Image Fragment Size:

`0 MB`

![Image Destination](screenshots/6.png)

### Step 7: Create Image

The source and destination information were displayed.

The option **Verify images after they are created** was selected.

Click **Start** to begin the acquisition.

![Create Image](screenshots/7.png)

### Step 8: Image Acquisition

FTK Imager started creating the forensic image from the physical drive.

![Creating Image](screenshots/8.png)

### Step 9: Image Verification

After acquisition, FTK Imager verified the created forensic image.

The verification process checks the integrity of the acquired image using hash values.

![Image Verification](screenshots/9.png)

### Step 10: Verification Result

The verification result showed:

- MD5 Verify Result: **Match**
- SHA1 Verify Result: **Match**
- Bad Blocks: **No bad blocks found in image**

![Verification Results](screenshots/10.png)

### Step 11: Image Summary

The image summary provided details about the acquired physical drive.

Important information included:

- Source Type: Physical
- Drive Model: SanDisk Cruzer Blade USB Device
- Drive Interface Type: USB
- Source Data Size: 59112 MB
- Sector Count: 121061376
- Bytes per Sector: 512

![Image Summary](screenshots/11.png)

### Step 12: Hash Verification

The image summary showed that the computed and reported hash values matched.

**MD5:**

`9f1f7659712cde7bc536dd82f341b5ce`

**SHA1:**

`abaca319c85c310078f410c02f6b11951af63334`

Both verification results were **Match**.

![Hash Verification](screenshots/12.png)

## Result

The physical USB drive was successfully acquired using **AccessData FTK Imager 4.7.1.2** and converted into a **Raw (dd) forensic image**.

The acquired image was successfully verified using MD5 and SHA1 hash values.

## Verification Results

| Parameter | Result |
|---|---|
| Image Type | Raw (dd) |
| Source | Physical Drive |
| Device | SanDisk Cruzer Blade USB Device |
| Source Size | 59112 MB |
| MD5 Verification | Match |
| SHA1 Verification | Match |
| Bad Blocks | No bad blocks found |

**Therefore, the forensic image was successfully created and its integrity was verified using MD5 and SHA1 hash values.**
<img width="171" height="121" alt="1" src="https://github.com/user-attachments/assets/4bae6b46-0ee9-43cc-90b5-dfddbfe33be3" />

<img width="171" height="121" alt="1" src="https://github.com/user-attachments/assets/c0a56ddd-c473-4d8f-835b-34a32a499ccd" />
