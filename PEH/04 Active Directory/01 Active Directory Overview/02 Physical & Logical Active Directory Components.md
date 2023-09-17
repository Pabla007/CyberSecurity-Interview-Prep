
![[Pasted image 20230826120048.png]]

<h2> Physical AD</h2>

>[!important] Very Important Active Directory Component is Domain Controller (i.e. It is the Head Honcho of all the Servers)
- It host our phone book (i.e. it has all the information on the User's , the Computer's or what printer's are in the Network etc.....)
- When we attack an internal network (i.e. it's very very bad if compromise your Domain Controller Cuz that means we can comprise the whole network)


Big Take away from Active Directory Data Stores is it holds a file name `Ntds.dit` (i.e. very sensitive file Cuz when we comprise a Domain Controller we will want to Grab this file)

>[!question] Why to Grab this File ?_?
Cuz it has Password Hashes of All the Users (i.e. we can take them offline and try to Crack them or can attempt Pass the Hash attack or attempt the Golden Ticket attack)

<h2> Logical AD</h2>

>[!question] What is Active Directory Schema ?_?
>- U can think of it as blueprint or rule book.


>[!question] What are Domains ?_?
Used to group things together.


>[!question] What are Tree's ?_?
It is a group of domains.
U have a parent and the children and they share namespace and they share some trust b/w them.


>[!question] What is a Forest ?_?
It is a collection of tree's.


Inside of a AD there are something called as Organizational Units (OUs)


>[!question] Trust ?_?
how we have access b/w resources 


>[!question] Lastly we have Objects ?_?
Objects is what is going to be inside of our Ous 



Domains -> Trees -> Forests -> Trust
     |
    V
  Ous -> Objects

