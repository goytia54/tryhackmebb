# Windows Fundamentals

## Windows Editions
* Started in 1985
* Windows XP, Vista, 7, 8.X, 10, 11

## File System
* Uses NTFS (New Technology File System)
* Before was FAT16/FAT32 (File Allocation Table)
* HPFS (High performance file system): used on usb devices and microSD cards

### NFTS
* Journaling file system
* Auto repair folders and files which uses FAT
* Supports files larger than 4GB
* Set specific permissions on folders and files
* File and folder compression
* Encryption via EFS (Encrpytion File System)

#### NFTS Permissions
* Full Control
* Modify
* Read & Execute
* List folder contents
* Read
* Write

#### Alternate Data Streams File Attribute
* At least one stream, $(DATA), per file
* Powershell allows you the ability to view these streams
* Can you ADS to hide data

## Windows System 32 Folders
* `C:\Windows` contains OS files
* `$windir$` is windows directory env variable
* `C:\Windows\System32` holds import ant window files in

## User Accounts, Profiles, and Permissions
* Can be administrator or standard user
* Command in run `lusrmgr.msd`

## User Account Control
* Administrator is prompted to give permissions to run programs

## Settings
* Primary place to make changes

## Control Panel
* Make more intense changes

## Task Manager
* [Blog Post](https://www.howtogeek.com/405806/windows-task-manager-the-complete-guide/)

## System Configurations
* MSConfig is for advance troubleshooting, to help and diagnose startup issues

### General Tab
* Select what devices and services for windows to load on boot
### Boot Tab
* Define boot options
### Services
* Special type of application that run in background

#### Computer Management Tool
* compmgmt
* System tools
  * Task Scheduler
  * Event Viewer: good for audit trail
  * Shared Folders
  * Local Users and Groups `lusrmgr.msc`
  * Performance: looking at performance of machine
  * Device Manager: Allow us to configure/disable hardware
* Storage
* Services and Applications

#### System Information
* msinfo32
* Gathers information about computer and displays a comprehensive manner
* Hardware Resources
* Components
* Software Environment: Contains enviromental variables
  
