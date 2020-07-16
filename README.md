# bginfo_teamviewer_id
Show your Teamviewer ID on the desktop with BgInfo.

PowerShell command (Run as Administrator):

(Get-ItemProperty -Path 'HKLM:\SOFTWARE\Wow6432Node\TeamViewer').ClientID | Out-File -FilePath c:\teamviewid.txt

Fetches the TeamViewer ID from registry and saves it into a .txt file.

-----------------------------------------------------------------------------------------------------------------

Navigate to "shell:startup". Create a new shortcut and add following:

C:\Users\mfi\bin\Bginfo64.exe config.bgi /timer:0 /nolicprompt /silent /taskbar

-----------------------------------------------------------------------------------------------------------------

bginfo-tm-id-custom-field.png

bginfo-tm-id.png
