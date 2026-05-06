# VM Tools

Install Command
``` cmd
setup.exe /S /v"/qn"
```

Uninstall Command
``` cmd
setup.exe /S /v "/qn msi_args REBOOT=R REMOVE=ALL"
```

Device Restart select:

**Intune will force a manatory restart**

![vmtools1](./media/vmtools1.jpg)

## Detection

Path: 

``` cmd
%ProgramFiles%\VMWare\
```

File or Folder: 

``` text
VMware Tools
```
![vmtools2](./media/vmtools2.jpg)

## Notes

To install only on VMWware Virtual Machines, you can create a group with dynamic device membership with the rules syntax as:
``` text
(device.deviceManufacturer -eq "VMware, Inc.")
``` 