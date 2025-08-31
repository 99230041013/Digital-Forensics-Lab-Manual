# Experiment 1 – Evidence Acquisition Using FTK Imager

**Objective:**  
To acquire volatile and non-volatile memory evidence using AccessData FTK Imager while ensuring data integrity.

---

## Description
FTK Imager is a forensic software by AccessData used for evidence acquisition and analysis. It can collect both **volatile memory (RAM)** and **non-volatile memory (hard disk, partitions, image files)**.

The tool can be used in two ways:
1. Portable version from USB/HDD (live acquisition).
2. Installed on investigator’s system (with source disk connected via write blocker).

---

## Volatile Memory Acquisition
- Open FTK Imager → select **Capture Memory**.  
- Options include capturing **pagefile.sys** and creating an **AD1 image file**.  
- Output: `.mem` file saved in the destination folder.  

---

## Non-Volatile Memory (Disk Image) Acquisition
- Open FTK Imager → **Create Disk Image**.  
- Supports sources: **physical drive, logical drive, image file, folder, CD/DVD**.  
- Supported formats:  
  - **RAW (dd):** Raw bitstream format.  
  - **SMART:** For Linux systems, supports compression.  
  - **E01:** Proprietary EnCase format with metadata and MD5 hash.  
  - **AFF:** Open-source Advanced Forensic Format (AFF4).  

**Steps:**  
1. Enter case details (examiner name, date, notes).  
2. Choose destination, image name, and fragment size (0 = single file).  
3. Select “Verify images after they are created” to ensure integrity.  
4. Start acquisition.  
5. Tool generates a text report with hash values.  

---

## Expected Output
- Volatile memory dump (`.mem`)  
- Disk image files (`.dd`, `.E01`, `.AFF`, etc.)  
- Hash verification report confirming evidence integrity  
