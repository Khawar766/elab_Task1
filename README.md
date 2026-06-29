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
For another test on linux machine with ip 192.168.100.189 running nmap -sS command
Note down IP addresses and open ports found.

For IP 192.168.100.189 1000 ports were scanned but all ports were filtered.  All scanned TCP ports are being filtered by a firewall or packet filter, so Nmap received no responses.
Optionally analyze packet capture with Wireshark.

Research common services running on those ports.

Identify potential security risks from open ports.
