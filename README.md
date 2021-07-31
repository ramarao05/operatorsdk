# operatorsdk instllation prereq in in Windows based linux Ubuntu
### Windows Subsystem Linux Enable Process::
### Open windows Power shell with admin priviliges (Task manager->File->type powershell and check the admin privilige check"
### dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
### Restart
### dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
### Restart
### Download "https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi" and install 
### if any permission errors , follow below steps:
### Turn windows features on or off --> uncheck the windows virtual machine and Windows subsystem for linux and reboot machine
### Turn windows features on or off --> check the windows virtual machine and Windows subsystem for linux and reboot machine (if the respective option available then use the above dism process)
### For Ubuntu::
### https://ubuntu.com/tutorials/ubuntu-on-windows###4-install-ubuntu-for-windows-10
### https://www.microsoft.com/en-us/p/windows-terminal/9n0dx20hk701?rtc=1&activetab=pivot:overviewtab
