Ticket: User Unable to Access Internet

Issue:
User reports being connected to Wi-Fi but unable to access any websites.

Environment:

Windows 10/11 workstation
Wireless network connection

Troubleshooting Steps Taken:

Confirmed issue affects multiple websites
Tested connectivity using ping 8.8.8.8 (successful)
Performed DNS lookup using nslookup google.com (failed)
Reviewed IP configuration using ipconfig /all
Identified potential DNS misconfiguration

Root Cause:
DNS resolution failure preventing domain names from resolving to IP addresses.

Resolution:

Executed ipconfig /release and ipconfig /renew
Flushed DNS cache using ipconfig /flushdns
Verified DNS resolution and restored internet access

Tools Used:

Command Prompt
ping
nslookup
ipconfig
