---
description: |
  Use the netcat (nc) tool to perform FTP banner grabbing and manually inspect the FTP service version on the target system. Netcat allows direct interaction with the FTP server for basic enumeration and banner retrieval.

  Command Reference:

      Target IP: 10.10.10.1

command: |
  nc -vn 10.10.10.1 21
items:
  - No_Creds
services:
  - FTP
OS:
  - Linux
  - Windows
  - Mac
attack_types:
  - Enumeration
references:
  - https://book.hacktricks.wiki/en/network-services-pentesting/pentesting-ftp/index.html
---
