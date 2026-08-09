# Experiment 1 – Evidence Acquisition Using AccessData FTK Imager

## Aim

To acquire a forensic disk image from a physical storage device using AccessData FTK Imager and to verify the hash values of the acquired image using MD5 and SHA1 algorithms.

## Software Used

1. AccessData FTK Imager 4.7.1.2

2. Windows Operating System

## Introduction

FTK Imager is a computer forensic software used for acquiring and analyzing digital evidence. The software can be used to acquire volatile memory as well as non-volatile memory, for example, hard disks and USB drives. In this experiment, acquisition of a physical storage device was performed and the evidence was exported in Raw (dd) forensic image format.

## Procedure

### Step 1: Launch AccessData FTK Imager 4.7.1.2

Launch AccessData FTK Imager 4.7.1.2 and select the option Create Disk Image from the welcome screen as shown below.

<img width="1033" height="657" alt="Screenshot 2026-08-09 230512" src="https://github.com/user-attachments/assets/f37863a7-9a10-4b8a-b6e6-cbf5a074dfe9" />




### Step 2: Select evidence source

The Select Source Window appeared as shown below.

<img width="340" height="275" alt="2" src="https://github.com/user-attachments/assets/c76dc85e-8f98-4dcb-a078-5f608d17b8e6" />


Select Physical Drive under Select Source and click Next.

### Step 3: Select Physical Drive

Select the physical drive from the list of available drives on the system and click Finish. The physical drive selected was SanDisk Cruzer Blade USB Device.

<img width="340" height="272" alt="3" src="https://github.com/user-attachments/assets/a1932725-bca5-456d-b725-310d00210461" />


### Step 4: Select Image Type

The Image Type Selection window appeared as shown below.



Select Raw (dd) as the desired image format and click Next. In this experiment, the Raw (dd) forensic image format was selected.

### Step 5: Enter Evidence Information

The window below appeared to enter the evidence details.

<img width="341" height="251" alt="5" src="https://github.com/user-attachments/assets/52f81dc1-5ac9-4bad-830e-8c2448830ad9" />



Enter the relevant case and evidence details. The following details were entered.

| Field | Details |

|---|---|

| Case Number | 1 |

| Evidence Number | 1 |

| Unique Description | DF |

| Examiner | SARATH KATURI |

| Notes | EXP 1 |

Click Next.

### Step 6: Select Image Destination

The window below appeared to select the image destination.

<img width="347" height="247" alt="6" src="https://github.com/user-attachments/assets/23134702-956e-4dd4-8e78-91eea4648dd8" />


Enter the desired image destination. The image destination selected was:

`D:\3-1\Digital Forensics`

Also, the image file name and image fragment size were selected. The imagefile name selected was: `diskimage` . Lastly, the image fragment size was set to `0` which implies that the image was not intentionally fragmented.

### Step 7: Configure image creation and verification options

FTK Imager displayed the selected evidence source and destination as shown below.

The option `Verify images after they are created` was enabled. This option ensured that the acquired image will be checked for reliability after acquisition.

<img width="351" height="299" alt="7" src="https://github.com/user-attachments/assets/493251dc-2058-4f04-a067-d5b8dbd59eb7" />



Click Start to begin the acquisition of the physical storage device image.

### Step 8: Create image

FTK Imager began acquiring data from the selected physical storage device and creating the image of the storage device.

<img width="309" height="221" alt="8" src="https://github.com/user-attachments/assets/c90a5a03-32fc-4943-85b0-f954aa2c366d" />



### Step 9: Verify acquired image

FTK Imager performed the verification process as shown below.

<img width="326" height="194" alt="9" src="https://github.com/user-attachments/assets/0633aac0-8a46-48fc-9ca7-4861f338f3c5" />



### Step 10: Display verification results

The verification results were displayed by FTK Imager as shown below.

<img width="959" height="272" alt="10" src="https://github.com/user-attachments/assets/77824455-2782-471c-8648-d78013c7a268" />



The results indicated that:

- The MD5 verification was a Match

- The SHA1 verification was a Match

- There were No bad blocks in the image

### Step 11: Image summary

The Image Summary displayed important details about the acquired image as shown below.

<img width="332" height="338" alt="11" src="https://github.com/user-attachments/assets/7cac7e56-d14a-4784-87f3-1b5fa8465ba3" />



The evidence acquisition details include:

| Parameter | Value |

|---|---|

| Source Type | Physical |

| Drive Model | SanDisk Cruzer Blade USB Device |

| Drive Interface | USB |

| Source Data Size | 59112 MB |

| Sector Count | 121061376 |

| Bytes per Sector | 512 |

### Step 12: View hash values

The final Image Summary displayed the hash values of the image as shown below.

<img width="310" height="322" alt="12" src="https://github.com/user-attachments/assets/f03816bc-d7c1-4395-ac79-421fea61bebe" />


The hash values were:

MD5 Hash: `9f1f7659712cde7bc536dd82f341b5ce`

SHA1 Hash: `abaca319c85c310078f410c02f6b11951af63334`

The computed and displayed hash values matched.

## Result

The physical storage device was acquired using the AccessData Forensic Tool. The acquired evidence was exported as a Raw (dd) forensic image. The integrity of the forensic image was verified using MD5 and SHA1 hashing algorithms. The results of the hash verification showed that both the MD5 and SHA1 hash values Matched and there were No bad blocks in the image.

## Conclusion

The experiment involved an acquisition of a physical storage device as a forensic image and verification of the integrity of the acquired image using hashing algorithms.
