---
title: "Windows Update With Powershell"
date: 2023-01-16
tags: [Windows]
image: "/images/how-to/windows-update-with-powershell/main.png"
type: "post"
showtableOfContents: true
---

**These actions are only possible with administrative privileges.*

## Prerequisites
Install the update module: 
```powershell
Install-Module PSWindowsUpdate
Add-WUServiceManager -MicrosoftUpdate
```

## Command
Install all availble updates 
```
Install-WindowsUpdate -MicrosoftUpdate -AcceptAll -AutoReboot | Out-File "C:\MSUpdates.log" -Force
```
Update logs can be found at: ```C:\MSUpdates.log```

![](/images/how-to/windows-update-with-powershell/2023.png)

that's it <3

----

{{< rawhtml >}} 
<script src="https://utteranc.es/client.js"
        repo="mansoorbarri/website"
        issue-term="title"
        theme="github-dark"
        crossorigin="anonymous"
        async>
</script>
{{< /rawhtml >}}