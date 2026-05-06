Links to MD files
``` powershell
Get-WmiObject -Class Win32_Product | Select Name, IdentifyingNumber
```
``` powershell
Get-WmiObject -Class Win32_Product | Where-Object {$_.Name -like "*NAME*"} | Select Name, IdentifyingNumber
```

* [Adobe Reader](/adobe-reader.md)
* [Fortinet FortiClient VPN](/fortinet-forticlient%20vpn.md)  **todo**
* [Google Chrome](/google-chrome.md)
* [Microsoft .Net enable](/microsoft%20.net%20enable.md)
* [Mozilla Firefox](/mozilla-firefox.md)
* [Netsweeper Client Filter](/netsweeper-client%20filter.md) **todo**
* [Netsweeper Wagent](/netsweeper-wagent.md) **todo**
* [VMWare Tools](./vmtools.md)


All intunewin files are stored in OneDrive, folder structure is as below:

* Publisher  
  *  Software
     * version

e.g.

* Google  
  * Chrome  
     * 147
     * 148
     * 149
* Mozilla  
  * Firefox  
     * 149
     * 150  