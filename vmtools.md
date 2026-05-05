# VM Tools

![vmtools1](./media/vmtools1.jpg)

Install Command
``` cmd
setup.exe /S /v"/qn"
```

Uninstall Command
``` cmd
setup.exe /S /v "/qn msi_args REBOOT=R REMOVE=ALL"
```

Device Restart select:

**Force Manatory reboot**

## Detection

Path: %ProgramFiles%\VMWare\
File or Folder: VMware Tools
