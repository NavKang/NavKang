## Windows Command Line
### Contents:

1. Ifconfig

2. Netstat

3. Ping

4. Tracert

5. ARP & Whoami
<br>
<hr>
#### Ifconfig:

+ ipconfig = current config  of installed IP stack
------------
+ ipconfig /all = detailed config report
------------
+ ipconfig /displaydns = detailed DNS report
---------------------------------------------

#### NetStat:

+ netstat = Displays active TCP connections and ports listening
------------
+ netstat -a = active conecctions
------------
+ netstat -no = displays top active connections
------------
+ netstat -ano = combo of above
------------
+ netstat -r = routing table
------------
+ Flags: -t -u -w -x =shows active TCP,UDP,RAW and Unix Socket connections- can combine with -a flag
------------
+ -s = displays statistics
+ -p = Tcp traffic
+ -f = FQDN format
+ -e = network interface statistics
+ -t(number of seconds) = time and number of seconds update
------------
+ netstat -an (time seconds) | find "port number" = checks every (seconds) and prints results if process start listening on Port 80
Enables us to watch the traffic with this command
------------

#### Ping:


+ Verifies IP level connecivity to another TCP/IP computer by sending an ICMP.
------------
+ ping, ping -t = continous
------------
+ ping -n (no. of pings) -l (no of bytes) <ip> = ping using number of  echo counts and size of bytes
------------

#### Tracert and route:

+ Tracert determines route to a destination by sending ICMP echo packets 
in these packets, Tracert uses varying IP TTL values.
------------
+ Route displays and modifies the enteries in local IP routing table which helps understand the topology of a network
------------
+ tracert -h (number) = specify max hops 
------------
+ route print = similar to netstat -r shows routing table
------------

#### ARP & whoami:


+ arp -a = Displays staticand dynamic entries to ARP cache table
------------
+ arp -av =as above but verbose mode
------------
+ arp -a -N <ip> = further details about specified interface IP
