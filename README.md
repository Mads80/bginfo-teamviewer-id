# bginfo_teamviewer_id
## Show your Teamviewer ID on the desktop with BgInfo.

PowerShell command: *(Run as Administrator)*
```powershell
(Get-ItemProperty -Path 'HKLM:\SOFTWARE\Wow6432Node\TeamViewer').ClientID | Out-File -FilePath c:\teamviewerid.txt
```

Fetches the TeamViewer ID from registry and saves it into a .txt file.

-----------------------------------------------------------------------------------------------------------------

Navigate to "shell:startup". Create a new shortcut and add following:

![BgInfo TeamViewer Id Shell Startup](bginfo-tm-id-shell-startup.png)

C:\Users\mfi\bin\Bginfo64.exe config.bgi /timer:0 /nolicprompt /silent /taskbar

-----------------------------------------------------------------------------------------------------------------

![BgInfo TeamViewer Id](bginfo-tm-id-custom-field.png)

![BgInfo TeamViewer Id Custom Field](bginfo-tm-id.png)
