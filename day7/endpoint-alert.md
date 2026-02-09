Summary:
Suspicious PowerShell execution detected on HR-LAPTOP-07 under user emma.johnson@company.com.

Reason for Alert:
PowerShell was executed with ExecutionPolicy Bypass and an encoded command originating from winword.exe, indicating possible macro-based malware execution.

Risk Level:
High

Assessment:
Encoded PowerShell commands executed from Microsoft Word are commonly associated with phishing-delivered malware. The behavior indicates an attempt to download and execute a remote payload.

Immediate Action:
Isolate the endpoint, terminate malicious processes, block the malicious URL, perform full malware scan, and reset user credentials.

Escalation:
Yes, escalate to L2 due to high-confidence malicious activity and potential system compromise.
