# Windows

## Use either Docker or VirtualBox
Open a Powershell window with admin privileges and execute either:

`bcdedit /set hypervisorlaunchtype off` for VirtualBox or 

`bcdedit /set hypervisorlaunchtype auto` for Docker and reboot the system.

## Install MinGW 64
https://winlibs.com/

[Source](https://stackoverflow.com/questions/61497394/installing-the-latest-version-of-mingw-w64-on-windows)