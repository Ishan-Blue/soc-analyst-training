Summary:
Multiple failed login attempts followed by a successful login were detected on the account john.doe@company.com at 01:42 UTC.

Reason for Alert:
Six failed authentication attempts occurred within four minutes, followed by a successful login from source IP 45.83.192.10, geolocated in Brazil. The legitimate user is based in Nepal, and the login was performed from an unknown device with no MFA triggered.

Risk Level:
High

Immediate Action:
Escalate to L2 SOC. Suspend the account, force password reset, terminate active sessions, block the source IP, and review post-login activity for potential compromise.
