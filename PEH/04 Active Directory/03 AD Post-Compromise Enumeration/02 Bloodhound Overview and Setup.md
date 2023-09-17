Command : apt install bloodhound

Username and Password : neo4j (i.e. Password changed to password)
![[Pasted image 20230828134235.png]]

Earlier we have to to download and set up it on the victim machine but now user can use it through kali Linux directly. 
- Invoke Bloodhound from Power Shell
- Tool called Sharp pound written in C sharp 

Search Invoke-Bloodhound GitHub in google
https://github.com/BloodHoundAD/SharpHound3
https://github.com/BloodHoundAD/BloodHound/blob/master/Collectors/SharpHound.ps1

Note all the 4 machine's should be running at this point (i.e. Windows Server and 2 Windows Pc along with Linux)
Simply copy and SharpHound.ps1 in The Punisher aka Frank Castle PC and run the script

![[Pasted image 20230828134751.png]]



![[Pasted image 20230828134446.png]]


![[Pasted image 20230828134534.png]]
But if we go to the queries we can see that they have some pre-built queries for us.

If we look at the Punisher.marvel that local administrator at Marvel.local has a session
here well i was logged in as Administrator so the sessions here.

>[!question] What does that make you think of ?_?
-Token Impersonation 
-Leverage attacks against this to try to compromise the administrator accounts with Mimi Katz.


>[!important] Enumeration Process never chances.....................
- Once we have an account on a network we're going to enumerate. 
- We're gonna try to find access once we get access.
- We are going to Re-enumerate we're going to see what information we can learn once we've gathered that account.

>[!note] Will talk about Post Compromise Attacks once we have compromised one account what can we do with that account and how can we leverage that into other compromises and eventually own this whole network here.

