# elab_Task1
Performing Task 1 for Elevate lab
Objective: Learn to discover open ports on devices in your local network to understand
network exposure
Install Nmap from official website.
Installing nmap using linux cmd command.
Find your local IP range 
Using command ip a my linux machine IP is 192.168.100.189
Run: nmap -sS 192.168.1.0/24 to perform TCP SYN scan.
Running the command nmap -sS 192.168.1.0/24
First discovered the open host, for 192.168.1.0/24,  then executed the command nmap -sS for open hosts, Nmap did not receive a response after the configured number of retransmissions, so it stopped probing that port. This typically indicates packet filtering by a firewall or another device that silently drops the probes.
For another test on linux machine with ip 192.168.100.189 running nmap -sS command
Note down IP addresses and open ports found.
When no response is received after all retries, Nmap treats the port as filtered, because it cannot tell whether the port is open behind a firewall or the packets were dropped.
For IP 192.168.100.189 1000 ports were scanned but all ports were filtered.  All scanned TCP ports are being filtered by a firewall or packet filter, so Nmap received no responses.
Optionally analyze packet capture with Wireshark.
Analyzing the packet using wireshark the target port is filtered (or the response was not captured), preventing completion of the TCP handshake.
Two packets together for TCP SYN scan against port 5906. The target immediately replied with RST, ACK, which means the port is closed. 

Research common services running on those ports.
Tested the IP but open ports were found all the ports were filtered or firewall dropping the packets. The output shows that Nmap is still not receiving responses from the target hosts, even after reducing the retry limit.
Nmap did not receive a response after the configured number of retransmissions, so it stopped probing that port. This typically indicates packet filtering by a firewall or another device that silently drops the probes.

I
