# Network scanning with NMAP

A port scanner is a computer program that checks network ports (virtual location where networking communication starts and ends) for one of three possible statuses – open, closed, or filtered.  There are two kinds of network ports on each computer (65,536 of each for a total of 131,082 network ports): TCP and UDP. A port scanner sends a network request to connect to a specific TCP or UDP port on a computer and records the response.

Port scanners are valuable tools in diagnosing network and connectivity issues. Attackers can use port scanners to detect possible access points for infiltration and to identify what kinds of devices you are running on the network, like firewalls, proxy servers or VPN servers. 

Port scanning  responses:

- Open, Accepted

- Closed, Not Listening

- Filtered, Dropped, Blocked

Port scanning techniques:

- Ping scan: looks for ICMP replies

- TCP Half open: requests ACK packet

- TCP Connect: Completes TCP connection

- UDP: Specific payload to target, like DNS request

- Stealth Scanning: Quiet and unobvious

## Common ports

- Telecommunication network protocol (Telnet): TCP port 23

- Secure Shell (SSH): TCP port 22

- Communications using DNS over the UDP protocol: TCP port 53

- Plaintext using SMTP: TCP port 25. 

- SMTP that uses TLS: TCP port 587. 

- POP3 cleartext: TCP port 110, 995 for encrypted

- IMAP: TCP 143 for plaintext and TCP 993 for IMAP over the encrypted TLS protocol

- SFTP (Secure File Transfer Protocol): TCP port 22. 

- File Transfer Protocol (FTP): TCP port 20, active mode data. The control process that tells the system which file to send usually communicates over TCP port 21.

- TFTP (Trivial File Transfer Protocol): UDP port 69.

- DHCP: UDP port 67 and UDP port 68

- HTTP: TCP port 80.  HTTPS: TCP port 443. 

- SNMP (Simple Network Management Protocol): UDP over port 161.

- syslog: UDP port 514 to send syslog data 

- Remote Desktop Protocol (RDP): TCP port 3389.

- NTP (Network Time Protocol): UDP port 123.

- Session initiation protocol: TCP port 5060 and TCP port 5061.

- Server Message Block (or CIFS, or the Common Internet File System): TCP port 445.

- LDAP (Lightweight Directory Access Protocol): TCP over port 389. LDAPS (Secure): TCP port 636.

- Microsoft SQL server (Microsoft Structured Query Language): TCP port 1433.

- Oracle’s SQLnet (Oracle Net or Oracle Net8): TCP port 1521. Open source database of MySQL: TCP port 3306.
