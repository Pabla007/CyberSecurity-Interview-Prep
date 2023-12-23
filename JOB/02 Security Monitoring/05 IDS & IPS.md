>[!question] What is IDS ?__?
- An IDS is an intrusion detection system as it can be a hardware appliance or a virtual machine.
- An IDS is a passive tool as it only monitors and reports and it's upto the security analysts to take the action.
![[Pasted image 20231026233209.png]]

- An IDS is generally packed at the edge of your network however if you would also like to monitor internal traffic, you can place inside the network as well.

>[!question] Function : And IDS operates based on signature or rules and some are also heuristic or behavior-based

![[Pasted image 20231026233530.png]]


IPS
An IPS is an intrusion prevention system that is active rather than passive.
It has the same basic architecture, rules and functions as an IDS but it will take action against the threat.

Anatomy of an IDS rule and will be using SNORT which is the most commonly used IDS.
![[Pasted image 20231026233906.png]]


sid has to be one million or higher cuz the first 999,999 are reserved for native snort rules.




WSUS Windows Server Update Services is a computer program and network service developed by Microsoft Corporation that enables administrators to manage the distribution of updates and hotfixes released for Microsoft products to computers in a corporate environment.