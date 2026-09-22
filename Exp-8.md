# Experiment 8 – Detection of Hidden Data Using StegExpose

## Aim

To use **StegExpose** to detect possible hidden or steganographic data in digital images.

## Software Requirements

- Java JDK
- StegExpose
- Windows PowerShell
- PNG image files

## Introduction

StegExpose is a steganalysis tool used to detect possible hidden information in images.

It analyzes statistical properties of images and identifies images that may contain hidden data.

In this experiment, StegExpose was used to analyze a folder containing PNG images.

---

## Step 1 – Open the StegExpose Folder

The StegExpose folder contains the `StegExpose.jar` file and the `testFolder` containing the images.

### Command

```powershell
cd "D:\3-1\Digital Forensics\Exp-8\StegExpose-master"
```

<img width="959" height="493" alt="1" src="https://github.com/user-attachments/assets/bd111485-4c14-465f-950a-5b4f0d5108dc" />


---

## Step 2 – Check the Test Images

The images available for analysis were verified using PowerShell.

### Command

```powershell
dir .\testFolder
```

The command displays the image files present inside the `testFolder`.

<img width="866" height="599" alt="2" src="https://github.com/user-attachments/assets/47d9e853-1fab-4066-a7c5-2884356d18d0" />


---

## Step 3 – Run StegExpose

StegExpose was executed on the `testFolder`.

### Command

```powershell
java -jar .\StegExpose.jar testFolder
```

The tool analyzed the images and identified three images as suspicious.



<img width="478" height="239" alt="3" src="https://github.com/user-attachments/assets/6604279e-fa26-4c54-aa37-a52bc9f16cba" />


---

## Step 4 – Save the Analysis Result

The StegExpose output was saved into a text file for documentation.

### Command

```powershell
java -jar .\StegExpose.jar testFolder > stegexpose_result.txt
```

The saved result was opened using Notepad.

### Command

```powershell
notepad .\stegexpose_result.txt
```

<img width="331" height="165" alt="4" src="https://github.com/user-attachments/assets/845d60f8-a186-4767-95e5-f6dd6f0d31dd" />


---

## Step 5 – Generate Detailed Analysis

A detailed CSV report was generated using a threshold value of `0.2`.

### Command

```powershell
java -jar .\StegExpose.jar testFolder default 0.2 stegexpose_detailed.csv
```

The generated CSV file contains detailed statistical information for the analyzed images, including whether each image was above the stego threshold.

### Command

```powershell
notepad .\stegexpose_detailed.csv
```

<img width="959" height="349" alt="5" src="https://github.com/user-attachments/assets/f72069cf-2f9b-493d-8f08-e6551b544847" />


---

## Step 6 – Analyze Using Threshold 0.3

StegExpose was also executed using a threshold value of `0.3`.

### Command

```powershell
java -jar .\StegExpose.jar testFolder fast 0.3
```

The same three images were identified as suspicious.

<img width="479" height="205" alt="6" src="https://github.com/user-attachments/assets/9ba52da5-d398-4899-9920-7496b6ff9f56" />


---

## Result

StegExpose successfully analyzed the images in the test folder and detected three suspicious PNG images.


The detailed CSV analysis also showed these three images as being above the selected stego threshold.

---

## Conclusion

Thus, **StegExpose was successfully used to detect possible hidden or steganographic data in digital images**. The tool analyzed the images and identified suspicious files based on their statistical characteristics.

