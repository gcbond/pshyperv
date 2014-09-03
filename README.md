# pshyperv
========

https://pshyperv.codeplex.com/


### PowerShell management Library for Hyper-V
A project to provide a PowerShell management library for Hyper-V 

It does pretty much what it says. Note that a lot of the information available from Hyper-V is only available if Powershell is running with Elevated privilege 
At present there are 80 functions in the library, some of these are worker functions which are not expected to be called directly, the others are listed below.

### _NOTE: The version of PSHyper-V available in the Source Code section is under active developement and is not guaranteed to be stable. If you require a stable release, please use one of the versions from the download area
### Finding a VM
Get-VM, Choose-VM , Get-VMHost

### Connecting to a VM
New-VMConnectSession

### Discovering and manipulating Machine states
Get-VMState , Set-VMState , Convert-VmState, 
Ping-VM , Test-VMHeartBeat, Shutdown-VM , Start-VM, Stop-VM, Suspend-VM
Get-VMKVP, Add-KVP, Remove-KVP, Get-VMJPEG

### Backing up, exporting and snapshotting VMs
Export-VM , Import-VM, Get-VMSnapshot, Choose-VMSnapshot , Apply-VMSnapshot , New-VMSnapshot ,Remove-VMSnapshot, Rename-VMSnapShot, Update-VMSnapshot, Get-VMSnapshotTree, Get-VmBackupScript

### Adding and removing VMs, configuring motherboard settings.
New-VM , Remove-VM , Set-VM , Get-VMCPUCount, Set-VMCPUCount, Get-VMMemory, Set-VMMemory, Set-VMSerialPort

### Manipulating Disk controllers, drives and disk images
Get-VMDiskController
Add-VMSCSIController , Remove-VMSCSIcontroller
Get-VMDriveByController , Add-VMDRIVE , Remove-VMdrive
Get-VMDiskByDrive, Add-VMDISK , Set-VMDisk, Get-VMDisk
Get-VMFloppyDisk , Add-VMFloppyDisk
Add-VMNewHardDisk

### Manipluating Network Interface Cards
Get-VMNic , List-VMNic , Choose-VMNIC, Add-VMNIC, Remove-VMNIC , Set-VMNICAddress , Set-VMNICConnection , Get-VMNicport , 
Get-VMnicSwitch, Choose-VMSwitch, New-VMSwitchPort, Get-VMByMACaddress, Choose-VMExternalEthernet,
New-VMExternalSwitch, New-VMInternalSwitch,New-VmPrivateSwitch

### Working with VHD files
Get-VHDDefaultPath, Get-VHDInfo, New-VHD, Compact-VHD, Test-VHD,Convert-VHD,Merge-VHD,Mount-VHD, Unmount-VHD
