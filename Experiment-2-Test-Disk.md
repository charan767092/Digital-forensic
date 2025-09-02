# Experiment-2: Recover Deleted or Damaged Files Using TestDisk

**Course / Lab:** Digital Forensics Lab  
**Experiment No.:** 2  
**Title:** Recover Deleted or Damaged Files Using TestDisk  

---

## Aim
To recover lost partitions and deleted files using TestDisk.

---

## Requirements
- TestDisk  
- Windows  

---

## Description
- TestDisk is an open-source forensic tool used for recovering lost partitions and repairing damaged boot sectors.  
- It can restore accidentally deleted files from FAT, NTFS, ext2/ext3 file systems.  
- Investigators use it to quickly recover inaccessible data and make disks bootable again.  

---

## Procedure — Steps to Recover Data Using TestDisk

**Step-1:** Launch the TestDisk tool. In the terminal window, select **Create** to make a new log file and press **Enter**. 

![(images/exp2-step1.png)](https://github.com/charan767092/Digital-forensic/blob/1ce68b26e468ab600296c8901050786681c7c977/images/IMG-20250902-WA0014%20-%20Copy.jpg)

**Step-2:** TestDisk will list available disks (HDDs, SSDs, USB drives). Use the arrow keys to highlight the disk you want to analyze and press **Enter**.  

![(images/exp2-step2.png)](https://github.com/charan767092/Digital-forensic/blob/1ce68b26e468ab600296c8901050786681c7c977/images/IMG-20250902-WA0017%20-%20Copy.jpg)

**Step-3:** TestDisk usually auto-detects the partition table (Intel/PC, EFI GPT, Mac, etc.). Verify and press **Enter**.  

![(images/exp2-step3.png)](https://github.com/charan767092/Digital-forensic/blob/1ce68b26e468ab600296c8901050786681c7c977/images/IMG-20250902-WA0018%20-%20Copy.jpg)

**Step-4:** Analyze the current partition structure. From the terminal, select **Analyse** and press **Enter**.  

![(images/exp2-step4.png)](https://github.com/charan767092/Digital-forensic/blob/1ce68b26e468ab600296c8901050786681c7c977/images/IMG-20250902-WA0020%20-%20Copy.jpg)

**Step-5:** After analysis, you will be asked to perform **Quick Search**. Select it and press **Enter**.  

![(images/exp2-step5.png)](https://github.com/charan767092/Digital-forensic/blob/1ce68b26e468ab600296c8901050786681c7c977/images/IMG-20250902-WA0019%20-%20Copy.jpg)

**Step-6:** TestDisk scans the disk and lists lost partitions.  

![(images/exp2-step6.png)](https://github.com/charan767092/Digital-forensic/blob/1ce68b26e468ab600296c8901050786681c7c977/images/IMG-20250902-WA0021.jpg)

**Step-7:** Press **P** to view the list of files and **C** to copy the files.  

![(images/exp2-step7.png)](https://github.com/charan767092/Digital-forensic/blob/1ce68b26e468ab600296c8901050786681c7c977/images/IMG-20250902-WA0025.jpg)

**Step-8:** If Quick Search does not find your partition/files, select **Deeper Search** and press **Enter**. This takes longer but finds more recoverable partitions.  

![(images/exp2-step8.png)](https://github.com/charan767092/Digital-forensic/blob/1ce68b26e468ab600296c8901050786681c7c977/images/IMG-20250902-WA0023.jpg)

**Step-9:** Once you are confident the partition is correct, select **Write** and press **Enter**.  

![Step 9](https://github.com/charan767092/Digital-forensic/blob/1ce68b26e468ab600296c8901050786681c7c977/images/IMG-20250902-WA0022.jpg)

**Step-10:** Confirm the operation by pressing **Y**. This will write the partition table to your disk.  

![Step 10](https://github.com/charan767092/Digital-forensic/blob/1ce68b26e468ab600296c8901050786681c7c977/images/IMG-20250902-WA0024.jpg)

- Once recovery is complete, exit TestDisk by selecting **Quit**.  
- Verify recovered files in the destination folder.  
- TestDisk detects lost or deleted partitions.  
- Files marked as deleted are listed and successfully copied to a safe location.  
- Recovery is possible without altering the original disk contents.  

---


