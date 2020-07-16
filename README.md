# bginfo_teamviewer_id

## Show your Teamviewer ID on the desktop with BgInfo.


Download BgInfo: https://docs.microsoft.com/en-us/sysinternals/downloads/bginfo

-----------------------------------------------------------------------------------------------------------------

PowerShell command: *(Run as Administrator)*
```powershell
(Get-ItemProperty -Path 'HKLM:\SOFTWARE\Wow6432Node\TeamViewer').ClientID | Out-File -FilePath c:\teamviewerid.txt
```

Fetches the TeamViewer ID from registry and saves it into a .txt file.

-----------------------------------------------------------------------------------------------------------------

Navigate to "*shell:startup*".

![BgInfo TeamViewer Id Shell Startup](bginfo-tm-id-shell-startup.png)

Create a new shortcut and add following:
```
C:\Users\mfi\bin\Bginfo64.exe config.bgi /timer:0 /nolicprompt /silent /taskbar
```
-----------------------------------------------------------------------------------------------------------------

Adding a Custom Field:

![BgInfo TeamViewer Id](bginfo-tm-id-add-custom-field.png)

End result:

![BgInfo TeamViewer Id Custom Field](bginfo-tm-id.png)
