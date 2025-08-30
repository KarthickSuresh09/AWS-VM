      THis REpostiory incomplete state  




 Id CommandLine
  -- -----------
   1 Get-Service W3SVC
   2 Get-NetFirewallRule | findstr HTTP
   3 Start-Service W3SVC
   4 netstat -ano | findstr :80
   5 Get-NetFirewallRule -DisplayName "*World Wide Web*"
   6 New-NetFirewallRule -DisplayName "Allow HTTP" -Direction Inbound -Protocol TCP -LocalPort 80 -Action Allow
   7 iisreset
