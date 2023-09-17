>[!question] What is a Kerberoasting attack?
It attempts to obtain a password hash of an Active Directory account that has a Service Principal Name (“SPN”).

Domain Controller is also known as a `key distribution center` (KDC):
Our user which need's to authenticate to the Domain Controller and when they do they are going to say that they request what is known as a Ticket Granting ticket aka NTLM hash

![[Pasted image 20230829124757.png]]
Any valid user (i.e. doesn't have to be admin) gets this ticket this is the authentication.
We have Fcastle and valid password Password1 which means valid tickey granting ticket.

>[!note] Will use GetUserSPNs from Impacket Tool kit.


![[Pasted image 20230829124818.png]]
So this service here has what is called SPN that is a service principal name.
KDC doesn't know that we have access to this server or not and provide us with TGS and this is where the Kerberoasting stops.