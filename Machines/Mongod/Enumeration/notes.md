nmap scan
```
$ nmap -sC -sV -A 10.129.146.154 -p-
Starting Nmap 7.94 ( https://nmap.org ) at 2023-07-16 20:33 CEST
Nmap scan report for 10.129.146.154
Host is up (0.029s latency).
Not shown: 65533 closed tcp ports (conn-refused)
PORT      STATE SERVICE VERSION
22/tcp    open  ssh     OpenSSH 8.2p1 Ubuntu 4ubuntu0.5 (Ubuntu Linux; protocol 2.0)
| ssh-hostkey: 
|   3072 48:ad:d5:b8:3a:9f:bc:be:f7:e8:20:1e:f6:bf:de:ae (RSA)
|   256 b7:89:6c:0b:20:ed:49:b2:c1:86:7c:29:92:74:1c:1f (ECDSA)
|_  256 18:cd:9d:08:a6:21:a8:b8:b6:f7:9f:8d:40:51:54:fb (ED25519)
27017/tcp open  mongodb MongoDB
| mongodb-databases: 
|   totalSize = 245760.0
|   ok = 1.0
|   databases
|     2
|       sizeOnDisk = 73728.0
|       empty = false
|       name = local
|     1
|       sizeOnDisk = 73728.0
|       empty = false
|       name = config
|     0
|       sizeOnDisk = 32768.0
|       empty = false
|       name = admin
|     4
|       sizeOnDisk = 32768.0
|       empty = false
|       name = users
|     3
|       sizeOnDisk = 32768.0
|       empty = false
|_      name = sensitive_information
| fingerprint-strings: 
|   FourOhFourRequest, GetRequest: 
|     HTTP/1.0 200 OK
|     Connection: close
|     Content-Type: text/plain
|     Content-Length: 85
|_    looks like you are trying to access MongoDB over HTTP on the native driver port.
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 81.52 seconds
```

