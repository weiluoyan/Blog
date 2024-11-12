# How to Install Ubuntu on Windows 10: A Step-by-Step Guide

Installing Ubuntu on Windows 10 is a straightforward process that requires creating a bootable USB drive and using it to install Ubuntu on your computer. Follow these steps to get Ubuntu up and running.

---

## Table of Contents

1. [Prerequisites](#prerequisites)
2. [Step 1: Download the Ubuntu ISO](#step-1-download-the-ubuntu-iso)
3. [Step 2: Download and Install a Bootable USB Tool](#step-2-download-and-install-a-bootable-usb-tool)
4. [Step 3: Insert the USB Drive and Open Disk Management](#step-3-insert-the-usb-drive-and-open-disk-management)
5. [Step 4: Create the Bootable USB Drive](#step-4-create-the-bootable-usb-drive)
6. [Step 5: Troubleshoot Common Issues](#step-5-troubleshoot-common-issues)
7. [Step 6: Boot from the USB Drive](#step-6-boot-from-the-usb-drive)
8. [Step 7: Install Ubuntu](#step-7-install-ubuntu)
9. [Additional Tips](#additional-tips)

---

## Prerequisites

- **USB Drive**: Minimum 8 GB capacity.
- **Ubuntu ISO**: Download from the [official Ubuntu website](https://ubuntu.com/download).
- **Bootable USB Tool**: Recommended tools are Rufus, Balena Etcher, or UNetbootin.

---

## Step 1: Download the Ubuntu ISO

1. Go to the [Ubuntu Downloads page](https://ubuntu.com/download).
2. Select your preferred version (Desktop or Server).
3. Download the ISO file to your computer.

---

## Step 2: Download and Install a Bootable USB Tool

- Choose one of these tools to create a bootable USB:
  - **Rufus**: [rufus.ie](https://rufus.ie)
  - **Balena Etcher**: [etcher.io](https://etcher.io)
  - **UNetbootin**: [unetbootin.github.io](https://unetbootin.github.io)

---

## Step 3: Insert the USB Drive and Open Disk Management

1. Insert your USB drive into a USB port on your computer.
2. *(Optional)* Open Disk Management by typing "Disk Management" in the Windows search bar.
3. Locate your USB drive and make sure it’s formatted (back up any important data).

---

## Step 4: Create the Bootable USB Drive

### Using Rufus

1. Open **Rufus** as an administrator.
2. Select your USB drive under **Device**.
3. Choose the Ubuntu ISO file by clicking **Select** under **Boot selection**.
4. Set **Partition scheme** to **MBR** and **Target system** to **BIOS or UEFI**.
5. Click **Start** to begin creating the bootable USB.

**Alternative: Using Balena Etcher**

1. Open **Balena Etcher**.
2. Click **Flash from file** to select the ISO.
3. Choose your USB drive as the target.
4. Click **Flash** to start.

---

## Step 5: Troubleshoot Common Issues

If you encounter issues with creating a bootable USB, try these fixes:

- **Reformat the USB Drive**: Use Disk Management to format it as **FAT32** or **NTFS**.
- **Assign a Drive Letter**: Use Disk Management to assign an unused drive letter.
- **Run as Administrator**: Run the bootable USB tool with admin privileges.
- **Try a Different USB Port or Drive**: Switching ports or drives can help.
![image](https://github.com/user-attachments/assets/8d744a60-4740-4b88-9af6-3f5dc8076c52)
![image](https://github.com/user-attachments/assets/3529e296-c0f4-45e5-a30e-9717f3d5965d)
![image](https://github.com/user-attachments/assets/72797510-86d2-40fc-b38e-c25d351cd241)
![image](https://github.com/user-attachments/assets/2aedb503-8dab-4fd8-b75b-20cf27d8633b)
![image](https://github.com/user-attachments/assets/31b5f143-7a38-470e-8f7b-971bd5791a17)
![image](https://github.com/user-attachments/assets/da299842-5ace-48b4-9cfb-0e0af5454f76)
![image](https://github.com/user-attachments/assets/e15d92ee-241c-4b5e-9c93-6224b4571708)
---

## Step 6: Boot from the USB Drive

1. Insert the bootable USB drive into the target computer.
2. Restart the computer and enter **BIOS/UEFI settings** (press F2, F10, F12, or Delete during boot).
3. Set the USB drive as the first boot device.
4. Save and exit BIOS settings.

---

## Step 7: Install Ubuntu

1. When the computer boots from the USB drive, the Ubuntu installer will open.
2. Choose **Try Ubuntu** to test or **Install Ubuntu** to proceed with installation.
3. Follow the prompts:
   - Select language, keyboard layout, and Wi-Fi connection (if needed).
   - Choose installation type (Erase disk, Install alongside Windows for dual-boot).
4. After installation, restart your computer, remove the USB drive, and start using Ubuntu.

---

## Additional Tips

- **Back Up Data**: Make sure to back up important files if you’re installing Ubuntu as your main OS.
- **Dual-Boot Option**: Select **Install alongside Windows** for a dual-boot setup.
- **Update System**: After installation, update Ubuntu by running `sudo apt update && sudo apt upgrade` in the terminal.

---


![image](https://github.com/user-attachments/assets/63b78439-6eaf-489e-ab6c-1f0636c4c146)
![image](https://github.com/user-attachments/assets/0771b903-e0ef-41bf-afa3-bc22832cb751)
![image](https://github.com/user-attachments/assets/0911f9c9-bfd3-49d7-86f1-e8cbb1310c6c)
![image](https://github.com/user-attachments/assets/8fe4b18f-3b84-401b-8122-a183467861a4)
![image](https://github.com/user-attachments/assets/9b17c62d-8c7f-4cc6-b072-1f98bbbcd64d)
![image](https://github.com/user-attachments/assets/c055ffdb-e319-4b10-93e4-b3bfe2678cbb)




**Happy Coding!**
