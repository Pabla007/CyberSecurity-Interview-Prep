
>[!question] What is Firewall ?__?
Firewall: is a network device that monitors and controls incoming and outgoing traffic.

Function:
Most basic feature of a firewall is Packer Filter at the Network Layer.

Stateful and stateless

What a firewall does not do ?_?
A firewall doesn't know if the traffic is good or traffic is bad.
It simply allows the traffic you tell it to allow, it denies the traffic you tell it to deny.
![[Pasted image 20231026225521.png]]

Why would a hacker want access to your specific network ?

A significant portion of internet traffic consists of automatedd bots, worms and general malware. Even if a hacker isn't after your company specifically, these automated threats have created a level playing field where we're all susceptible to attack.


Where does Firewall fit in our three component model of security ?
It has all three - prevention , detection and response

CISCO / PALO ALTO 
Next Gen Firewall: is a network security device that provides capabilities beyond a traditional, stateful firewall as a next-generation firewall includes additional features like application awareness and control, integrated intrusion prevention, and cloud-delivered threat intelligence.

NGFW is perfect for automation. They allow you to subscribe to automatic threat lists such as IP and URL blacklists that are updated dynamically based on intelligence.

The NGFW will use the application instead of a port, for example, SSH instead of TCP-22 as the built-in intelligence can detect if it is indeed SSH traffic and not just TCP-22 traffic.


![[Pasted image 20231026230124.png]]
Access-list : This is a rule that controls trffic
Acme-Ingress : the name of our internal interface
Extended permit : flexibility in matching traffic and the ability ot match based on protocol, source and destination address
Source: always goes first 
Destination: always after the source
Eq: means 'equal to' and 9081 is the port required above



Intrusion Detection System: is a device or application that monitors traffic for malicious activity or policy violations.