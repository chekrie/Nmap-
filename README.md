# Nmap-
┌──(kali㉿kali)-[~]
└─$ nmap -sS 172.20.10.3  
Starting Nmap 7.95 ( https://nmap.org ) at 2025-09-22 02:20 EDT
Nmap scan report for 172.20.10.3
Host is up (0.0057s latency).                                                                                                          
Not shown: 992 filtered tcp ports (no-response)                                                                                        
PORT     STATE SERVICE                                                                                                                 
80/tcp   open  http                                                                                                                    
135/tcp  open  msrpc                                                                                                                   
139/tcp  open  netbios-ssn                                                                                                             
445/tcp  open  microsoft-ds                                                                                                            
3306/tcp open  mysql                                                                                                                   
5357/tcp open  wsdapi                                                                                                                  
8000/tcp open  http-alt                                                                                                                
8089/tcp open  unknown

Nmap done: 1 IP address (1 host up) scanned in 6.01 seconds

┌──(kali㉿kali)-[~]
└─$ nmap -sU 172.20.10.3

Starting Nmap 7.95 ( https://nmap.org ) at 2025-09-22 02:27 EDT
Stats: 0:05:58 elapsed; 0 hosts completed (1 up), 1 undergoing UDP Scan
UDP Scan Timing: About 66.15% done; ETC: 02:36 (0:03:03 remaining)
Stats: 0:06:50 elapsed; 0 hosts completed (1 up), 1 undergoing UDP Scan
UDP Scan Timing: About 78.05% done; ETC: 02:35 (0:01:55 remaining)
Nmap scan report for 172.20.10.3
Host is up (0.0015s latency).
Not shown: 988 filtered udp ports (port-unreach), 4 filtered udp ports (net-unreach)
PORT     STATE         SERVICE
137/udp  open|filtered netbios-ns
138/udp  open|filtered netbios-dgm
1900/udp open|filtered upnp
3702/udp open|filtered ws-discovery
4500/udp open|filtered nat-t-ike
5050/udp open|filtered mmcc
5353/udp open|filtered zeroconf
5355/udp open|filtered llmnr

Nmap done: 1 IP address (1 host up) scanned in 512.48 seconds


┌──(kali㉿kali)-[~]
└─$ nmap -sn 172.20.10.3
Starting Nmap 7.95 ( https://nmap.org ) at 2025-09-22 02:38 EDT
Nmap scan report for 172.20.10.3
Host is up (0.0042s latency).
Nmap done: 1 IP address (1 host up) scanned in 0.17 seconds

I explored network reconnaissance and security analysis using Nmap. I began by installing and configuring the tool, then performed TCP SYN scans across my local network to identify active hosts and open ports. I documented the results, researched the common services associated with those ports, and analyzed potential security risks that could arise from exposed services
and what am trying to scan entire network its taking long time instead of that i have tries others scan
