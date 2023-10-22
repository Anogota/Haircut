```
Starting Nmap 7.93 ( https://nmap.org ) at 2023-10-22 12:45 CEST
Nmap scan report for 10.10.10.24
Host is up (0.084s latency).
Not shown: 65533 closed tcp ports (conn-refused)
PORT   STATE SERVICE VERSION
22/tcp open  ssh     OpenSSH 7.2p2 Ubuntu 4ubuntu2.2 (Ubuntu Linux; protocol 2.0)
| ssh-hostkey: 
|   2048 e975c1e4b3633c93f2c618083648ce36 (RSA)
|   256 8700aba98f6f4bbafbc67a55a860b268 (ECDSA)
|_  256 b61b5ca9265cdc61b775906c88516e54 (ED25519)
80/tcp open  http    nginx 1.10.0 (Ubuntu)
|_http-server-header: nginx/1.10.0 (Ubuntu)
|_http-title:  HTB Hairdresser 
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel
```
Nic ciekawego
Zrobilem content discovery i tutaj jest tylko /uploads
```
[####################] - 43s    59998/59998   0s      found:1       errors:0      
[####################] - 43s    29999/29999   691/s   http://10.10.10.24/
[####################] - 43s    29999/29999   692/s   http://10.10.10.24/uploads
```
