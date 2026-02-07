Summary:
Multiple failed login attempts followed by a successful login detected on user account michael.brown@company.com at 03:26 UTC.

Reason for Alert:
Five failed authentication attempts were observed within a 3-minute window, followed by a successful login on the sixth attempt.
The login originated from an IP address not previously associated with the user.

Risk Level:
Medium

Investigation Details:
- Affected User: michael.brown@company.com
- Failed Attempts: 5
- Successful Attempt: 1
- Source IP: 103.214.92.44
- Geolocation: Vietnam
- Legitimate User Location: Nepal
- Device: Unknown
- MFA Status: Not triggered

Assessment:
The login behavior indicates a possible password spraying or brute-force attempt that resulted in successful authentication.
The source location and device do not match the user's normal login patterns.

Immediate Action:
- Force password reset for the affected account
- Revoke active sessions
- Enable MFA for the user account
- Escalate to L2 SOC for further investigation

