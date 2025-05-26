# CyberSecurity
#NMAP:- USED FOR ACTIVE RECONNAISSANCE WHICH INCLUDES VULNERABILITY SCANNING AND NETWORK MAPPING
#FOR HOST AND PORT SCANNING
firstly scan nmap subnet with local ip to check which host is up or down (nmap -sn 127.0.0.1/8)
default scan to 1000 ports (nmap 127.0.0.1)
scan for all 65535 ports (nmap -p- 127.0.0.1)
scan for specific ports 80-http 443-https (nmap -p 80,443 127.0.0.1)
#FOR SERVICE SCANNING
scan which service/version running is the open ports (nmap -sV 127.0.0.1)
#FOR OS DETECTION
it scan which os is currently used and version of it (sudo nmap -O 127.0.0.1)
#AGGRESSIVE SCAN INCLUDE OS, VERSION AND SCRIPIT SCANNING
    (nmap -A 172.0.0.1)
#SCAN TYPES
-sS SCAN used for send syn packets to target (nmap -sS 172.0.0.1)
-sT uses full TCP connection 3-way handshake (nmap -sT 172.0.0.1) 9 -sU scans udp ports (nmap -sU 172.0.0.1)
-sA used to mapp firewall rules (nmap -sA 172.0.0.1)
-sN sends TCP packet with no flags set (nmap -sn 172.0.0.1)
-sS command is used to send the SYN packet to the target if the target is up and ready to connect it send SYN+ACK packet it means target is ready to connect, if it sends only SYN packet then it means target is down.
