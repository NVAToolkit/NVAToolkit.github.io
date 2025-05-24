---
description: |
  Use the nmap tool to perform FTP banner grabbing and identify the FTP service version on the target system. Nmap automates service detection and helps gather information about the FTP server for further enumeration and assessment.

  Command Reference:

      Target IP: 10.10.10.1

command: |
  nmap -Pn -p 21 -sV 10.10.10.1
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
