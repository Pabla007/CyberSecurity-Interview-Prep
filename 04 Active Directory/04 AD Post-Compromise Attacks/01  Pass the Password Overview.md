>[!question] What is Pass the Hash/Password ?__?
Pass the Hash attack is technique where an attacker captures a password hash and than passes it through for authentication and lateral access.

Tool that we're going to use called **"crackmapexec"**
Passing the Password using CrackMapexec
![[Pasted image 20230829105030.png]]

Simply get a Shell using Psexec using MSFConsole or through Psexex.py :
![[Pasted image 20230829105117.png]]

So playing off the different example for pass the hash let's say that we have a "psexec"
here which we get on to this machine and we run a hash stump.

Will take the hash dump of FCastle as shown in the figure and capture the last bit (i.e. NTLM hash) and will try to pass that around.
User : Fcastle which is a local user.
>[!important] As u can see we didn't have any luck on this one but these local accounts are very dangerous. 

Local account don't have the `lockedout policy` like domain accounts do.
The issue is a lot of administrator will reuse the same account and password to set up machines. 
>[!important] So looking into these local hashes/ these local accounts are super important as well.


