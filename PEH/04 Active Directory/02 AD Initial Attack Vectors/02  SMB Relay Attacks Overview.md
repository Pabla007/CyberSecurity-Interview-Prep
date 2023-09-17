>[!question] What is SMB Relay ?__?
>- It stands for Server Message Block, a network file-sharing protocol that operates on the Application and Presentation Layers, but heavily reliant on lower-level protocols.
>- Hashes are being relayed to specific machines to potentially gain access.


![[Pasted image 20230827200731.png]]
**Requirements :**
1st requirement
SMB signing is to be disabled on the target. (i.e. SMB is a packet level protocol)
- If SMB signing is enabled when we tried to relay credentials it will say Hey you are not really that person cuz the packet is not signed by you and i not gonna let you in.
- But if SMB signing is Disabled than it never checks. (i.e. it never checks for **authenticity** of where this is coming from (i.e. there's the user there's the Hash and they have the permissions to do so)

2nd Requirement 
- User Being relayed has to have admin rights credentials on that machine.
We cannot relay a credential that we captured from one machine back to the same machine (i.e. say we are dot 6 we can't relay that credentials to dot 6)
This has to be done on 2 separate machines.


![[Pasted image 20230827200949.png]]
- Will change the setting in the responder file (i.e. will turn off the SMB and HTTP)
- Will going to be listening and not responding on this server.

The Server Message Block uses TCP port 445 for connection and, of course, data transmission. If the resource requested is located on the web, the address resolution is handled through the DNS. 
https://heimdalsecurity.com/blog/what-is-an-smb-relay-attack/

>[!note] Responder to Capture and another tool to relay (i.e. psexec.py)

![[Pasted image 20230827201413.png]]
It will take the relay and passes that to the Target file (i.e. But how to identify the Target file)


![[Pasted image 20230827201612.png]]
We point to machine with responder listening and it can't access the machine.
DNS fails and responder kicks in and doesn't responds to that message and relay the credentials to this other machine.


![[Pasted image 20230827201654.png]]
Think as SAM the Shadow of the Windows world (i.e. user and hashes of the local users and not the domain users.)
But we can take down the entire network with local users.
So we will not only dump the hashes but also get the shell. 
