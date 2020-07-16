# bginfo_teamviewer_id
Show your Teamviewer ID on desktop with BgInfo.

PowerShell command (Run as Administrator):

(Get-ItemProperty -Path 'HKLM:\SOFTWARE\Wow6432Node\TeamViewer').ClientID | Out-File -FilePath c:\teamviewid.txt

Fetches the TeamViewer ID from registry and saves it into a .txt file.
