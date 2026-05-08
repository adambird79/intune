# Enable Microsoft .Net 3.5 

Create a powershell script to enable the feature

``` powershell enable_Net3.5.ps1
Enable-WindowsOptionalFeature -Online -FeatureName NetFx3
```

Also create a powershell script to disable the feature

``` powershell disable_Net3.5.ps1
Disable-WindowsOptionalFeature -Online -FeatureName NetFx3
```

Install command: powershell.exe -WindowStyle hidden -ExecutionPolicy ByPass -File enable_Net3.5.ps1
Uninstall command: powershell.exe -WindowStyle hidden -ExecutionPolicy ByPass -File disable_Net3.5.ps1
