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

4. Select the partition table type (usually detected automatically). 

<img width="975" height="509" alt="Image" src="https://github.com/user-attachments/assets/2b779df0-e07d-43fb-801f-682bd892e280" />
 
5. Run **Analyze** to search for lost partitions.  
6. Choose **Quick Search** or **Deeper Search** based on results.  
7. Highlight the lost partition(s) → press Enter to continue. 

<img width="772" height="528" alt="Image" src="https://github.com/user-attachments/assets/e2758c75-b5b7-42db-bea3-a731c243c983" />
 
8. Write the partition structure to disk.  
9. Reboot the system to apply changes.

---

## Expected Output
- Recovery of deleted partitions.  
- Restored access to lost files.  
- A session log file containing recovery details.  

<img width="724" height="447" alt="Image" src="https://github.com/user-attachments/assets/6dbe43b1-4ea7-4ba0-a5db-fc2ae4eb063a" />
