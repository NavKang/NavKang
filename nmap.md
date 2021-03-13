### NMAP Commands
-iL    : List scan

-sS   : SYN scan

-p    : Requests all port scan, instead of 1024 default

-A    : Agreesive & Aadvanced inc OS & Service detect

-P    : Ping scans (+ specify ports)checks availability
Flags:   -PS - Syn, -PA - Ack, -PU - UDP, -PE

-PN   : Scans all ports, available or not

-sL -n  : List scan with no reverse DNS resolution

-n    : no resolution

-R    : all resolution

--traceroute : traceroute

--script -sC : NSE scripting

<br>
### Further Details and Usage:
<br>

1. nmap --iflist  =displays IP/Mask for each device connected to NW
--------------------
2. nmap -F     =fast scan
--------------------
3. nmap -sP =ping scan
--------------------
4. nmap --reason <ip> = ports and port state, provides reason info of a  syn ack pack ussing TTL of 128
--------------------
5. nmap --open <ip> = displays open ports only (0-65535)
--------------------
6. nmap -p <port> <ip> =specific port scan 
--------------------
7. nmap -p T:<port> <ip> =specifies either TCP/UDP mode for port
--------------------
8. nmap --packet-trace <ip> =traces packet
--------------------
9. nmap -sA <ip> =identifes and scans firewall protected host/NW
--------------------
10. nmap -PN =scans every IP (online or offline)
--------------------
11. nmap -PS =scan using TCP,SYN and ACK ping (empty TCP pack with SYN flag set) -default port=80, to change -PS<port> nospace
--------------------
12. nmap -PA =uses ACK flag in 3wayHS, purpose to acknowledge data over a  supposed connection where none exists
--------------------
13. UDP scanning - UDP ping scans have advantage of being capable of detecting systems behind firewalls with strict TCP filtering leaving UDP traffic forgotten.
--------------------
14. nmap -sP -PU <ip> = assists with tracking UDP pings used for bypassing firewalls
--------------------
15. nmap -O <ip> = OS detection
--------------------
16. nmap -v <ip> = verbose scan, detailed info
--------------------
17. nmap -v -O --osscan-guess <ip> = combined scan, OS guess
--------------------
18. nmap -sV <ip> = use when we suspect a system that might hold remote services
--------------------
19. nmap -PO <ip> 
--------------------
20. nmap -sU <ip> = UDP scan
--------------------
21. nmap (ip) >(filename).txt =output results to txt
-------------------  

can use -oN and -oG for GREP -oX for XML (preferred for scripts and programs that process NMAP results)
