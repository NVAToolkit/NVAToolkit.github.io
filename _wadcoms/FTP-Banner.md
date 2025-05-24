---
description: |
  Perform FTP banner grabbing to identify the FTP service version and gather information about the target system. This can be achieved using tools like nmap for automated service detection, netcat (nc) for manual inspection, or openssl for checking encrypted FTP connections. Banner grabbing is a fundamental enumeration technique that helps assess potential vulnerabilities and tailor further penetration testing steps.

  Command Reference:

      Target IP: 10.10.10.1

command: |
  nmap -Pn -p 21 -sV 10.10.10.1

  nc -vn 10.10.10.1 21

  openssl s_client -connect 10.10.10.1:21 -starttls ftp
items:
  - No_Creds
services:
  - FTP
OS:
  - Linux, Windows, Mac
attack_types:
  - Enumeration
references:
  - https://book.hacktricks.wiki/en/network-services-pentesting/pentesting-ftp/index.html
---
