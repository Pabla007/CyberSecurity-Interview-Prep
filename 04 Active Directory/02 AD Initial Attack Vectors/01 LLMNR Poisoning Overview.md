>[!question]  So what is LLMNR ?_?
link local multicast name resolution used to identify hosts when DNS fails to do 

![[Pasted image 20230827192613.png]]

![[Pasted image 20230827192838.png]]


The server Name is Hackme and the user by mistake writes `hackm` which caused a DNS issue 
So will send a broadcast message if anyone knows about it. And we who are listening in the network (i.e. Man In The Middle Attack)
So this is what LLMNR is we are listening in the middle and the request happens we are just waiting for a response to happen (i.e. user name and hash)
Will run a tool called **RESPONDER**

>[!note] Responder is a part of IMPACKET tool kit.

>[!important] Mentor's Strategy:
Always run this tool first in the morning or right after lunch Cuz as u need a lot of traffic (i.e. Start this before any Nmap scans or Nessus etc....)

Running Responder :
![[Pasted image 20230827192942.png]]

Somebody entered a wrong network drive (i.e. Failed to do DNS) 
