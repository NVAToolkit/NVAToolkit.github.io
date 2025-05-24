---
description: |
  Use the openssl tool to perform FTP banner grabbing and inspect the FTP service version over an encrypted connection. Openssl allows you to initiate a STARTTLS session with the FTP server for secure enumeration and banner retrieval.

  Command Reference:

      Target IP: 10.10.10.1

command: |
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