https://www.vulnhub.com/

>[!question] :What is a ARP-scan ?_?
It is a command-line tool which uses ARP protocol (i.e. PLUG and PLAY Address Resolution Protocol that connects an IP to MAC) to discover as well as fingerprint IP hosts on the local network.

```
Command : apr-scan -l
```

<h2>Nmap </h2>

```
command : nmap -T4 -p- -A <IP address>
```

where
- -T4 is the speed preference given by Nmap and will use T4
- -p- means will scan for all the port out there.... But if we use -p it will scan the top 1000 ports for us. We can also specify port like 80,443,53 etc...
- -A stands for everything which means it will give us everything that's available out there (i.e OS version , Finger printing etc...)

```
command : nmap -sU -T4 --top-ports 1000 192.168.142.129
```
as UDP is connection less so it will take forever to run so will specify to scan only the top 1000 ports in this case.

There are many scanning options but will mostly use ping sweep (A ping sweep (also known as an `ICMP sweep`) is a basic network 
scanning technique used to determine which of a range of IP addresses map to live hosts (computers). ), 

>[!question] :What is Stealth Scanning ?__?
Stealth scan types are those where reset flags cause the target system to respond without having a fully established connection.

3-Way Handshake:- We know the concept of 3 Way Handshake where we used to scan for open port's and connect with them (i.e. SYN SYNACK ACK)
- Will do the same thing but with nmap (i.e. Network Mapper)
command: SYM SYNACK RST nmap -sS
WHICH is called as `Stealth scanning` as it used to be Stealthy but not anymore.
- But still Nmap don't get picked up at 80% of the pen-testing


>[!important] :- SYN SYNACK RST
Will tell google make a connection and it will reveal us the port that is open than will send the reset flag (i.e. Just kidding don't want to make a connection)



It our job to look for the information on the OPEN ports and find which are the certain ports to attack first and how to enumerate everything.

TCP SYN (Stealth) Scan (-sS)
nmap -sS -T4 -A <IP address>

Will use this when Stalth was not an option
TCP Connect Scan (-sT)
nmap -sT -T4  -A <IP address>
SYN 
SYN ACK
ACK
Data
RST