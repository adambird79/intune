# Enable Microsoft .Net 3.5 

Create a powershell script to enable the feature

enable_NetFx3.ps1
``` powershell enable_NetFx3.ps1
Enable-WindowsOptionalFeature -Online -FeatureName NetFx3
```

Also create a powershell script to disable the feature

``` powershell disable_NetFx3.ps1
Disable-WindowsOptionalFeature -Online -FeatureName NetFx3
```

Install command: powershell.exe -WindowStyle hidden -ExecutionPolicy ByPass -File enable_NetFx3.ps1
Uninstall command: powershell.exe -WindowStyle hidden -ExecutionPolicy ByPass -File disable_NetFx3.ps1

Create a detection script as below
``` powershell
$Enabled = Get-WindowsOptionalFeature -online | Where FeatureName -eq 'NetFx3' | Select -expandproperty State
If ($enabled -eq "enabled") {
Write-Output ".net 3.5 is enabled"
Exit 0
}
Else {
Write-Output ".net 3.5 is not enabled"
Exit 1
}
```



