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

#### Resource Monitor
* resmon
* Advanced resource monitoring

#### Command Prompt
* cmd
* Example commands
  * `hostname`: computer name
  * `whoami`: logged in user
  * `ipconfig`: command will show the network address settings
  * `/?` is the like manual for commands
  * `cls` clear command prompty
  * `netstat` displays protocol statistics for TCP/ICP
  * `net` by itself is a command with many options, can run with `net help`

#### Windows Registry
* regedit
* Central database used to store info needed to configure system, application and hardware devices

## Windows Update
* Provides security updates, feature enhancements, and patches for OS and other products such as defender
* `control /name Microsoft.WindowsUpdate`

## Windows Security
* Available in settings
* Various protection areas
   * Virus and threat protection
   * Firewall and network protection
   * App & Browser control
   * Device security

### Virus & Threat Protection
* Current Threats
  * Scan Options
     * quick scan: check where threats are usually found
     * full scan: all computer scan
     * custom scan: choose files
  * Threat History
     * last scan
     * quarantined threats
     * allowed threats
  * Virus & threat protection settings
     * real time protection - locates and stops malware from installing or running on your device
     * cloud delivered protection: latest protection from information from the cloud
     * automatic sample submission: send samples to microsoft to help them defend
     * controlled folder access: protect files and folders
     * Exclusions: anti virus won't scan here
     * Notifications: windows defender antivirus will sent notifications
  * Ransomeware protection
     * controlled folder accesss

### Firewall Protection
* Control whats comes in and out of the ports
* Have many firewall profiles

#### Domain
* networks where the host system cna authenticate to a domain controller
#### Private
* User assigned profile
#### Public
* Public profile for public networks

### App & Browser Control
* Microsoft Defender SmartScreen
  * Protects against phising or malware websites/applications and downloading bad files
 
### Device Security
* Core isolation: memory integrity, prevents malicious code into high security processes
* Security Processor: Trusted Platform Module, allowing for additional encryption

## BitLocker
* Drive encryption to prevent data theft or exposure from lost or stolen computers

