## Make Bootable Drive

1.  Begin by downloading Rufus, (https://rufus.ie/en/)a software tool for creating bootable drives.
    
2.  Before proceeding, determine the partition type of your hard disk, which can be either GPT or MBR.
    
3.  If your hard disk utilizes the GPT (GUID Partition Table) partition style, proceed with the following settings in Rufus:
    
    a. Choose "GPT" as the partition scheme.
    
    b. Ensure that the target system is set to "UEFI (non CSM)."
    
4.  In Rufus, select the Linux ISO file you want to use as the bootable operating system in the "Boot Selection" or "Bootable Disk Image" section.  
![Alt text](https://drive.google.com/file/d/1sRl0B5DgEkEtLiRJGd5p4mpLN908AZWY/view?usp=sharing)



* * *

## Disk Partition

This is a sample partition scheme for a 500GB storage.2.

### 1\. EFI

==Give space:== 1025 MB

==Type of new partition==: Primary

==Location:== Beginning of the space

==Use as==: EFI System Partition

### 2\. Swap

==Give space==: 16 GB $\approx$ 16,000 MB (To double the RAM, if it is 8 GB, increase it to 16 GB, and if it is 4 GB, increase it to 8 GB.)

==Type of new partition==: Primary

==Location:== Beginning of the space

==Use as:== Swap Area

### 3\. (/) Root

==Give space==: 190 GB $\approx$ 190464 MB

==Type of new partition==: Primary

==Location==: Beginning of the space

==Use as:== Ext4 Journaling File System

==Mount point==: (/)

### 4\. /home

==Give space==: 293GB $\approx$ 292134 MB

==Type of new partition==: Primary

==Location:== Beginning of the space

==Use as==: Ext4 Journaling File System

==Mount Point==: /home

* * *

Here is the picture  
![Alt text](https://drive.google.com/file/d/1_yT2LN0Z_phV-qYwL7zFsBDpNWdpBrMC/view?usp=drive_link)
    
