# Experiment 2 – TestDisk

**Objective:**  
To recover lost partitions and repair corrupted file systems using TestDisk.

---

## Description
TestDisk is an open-source forensic tool designed for data recovery and disk repair.  
It can recover lost partitions, make non-booting disks bootable again, and restore files from deleted or damaged partitions.

Supported tasks include:
- Recovering lost partitions
- Rebuilding boot sectors
- Repairing file tables
- Copying deleted files

---

## Procedure
1. Launch TestDisk (run as administrator).  
2. Select **Create New Log File** to document the session.

<img width="970" height="530" alt="Image" src="https://github.com/user-attachments/assets/7b311b80-4ac1-4029-b251-8757bc36b5c7" />
  
3. Choose the affected disk.  

<img width="970" height="530" alt="Image" src="https://github.com/user-attachments/assets/7b311b80-4ac1-4029-b251-8757bc36b5c7" />


4. Select the partition table type (usually detected automatically).  
5. Run **Analyze** to search for lost partitions.  
6. Choose **Quick Search** or **Deeper Search** based on results.  
7. Highlight the lost partition(s) → press Enter to continue.  
8. Write the partition structure to disk.  
9. Reboot the system to apply changes.

---

## Expected Output
- Recovery of deleted partitions.  
- Restored access to lost files.  
- A session log file containing recovery details.  

---

## Output Screenshots
![Partition Analysis](screenshots/testdisk-analysis.png)  
*Figure 1: Analyzing disk for lost partitions using TestDisk*  

![Partition Recovery](screenshots/testdisk-recovery.png)  
*Figure 2: Partition successfully recovered with TestDisk*  
