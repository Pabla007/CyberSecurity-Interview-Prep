SMB (Server Message Block): Port 445 (TCP)
Think of it as file share
Originally it was 139 and in later version of windows they put on 445
Also know as `Samba`
WannaCry Virus also known as EternalBlue - MS17-010

<h2> Metasploit</h2>
- SMB is a file share which is commonly used in work environment and internal environment.
- We think of a attack (i.e. MS 17010) which is the latest and the greatest of all.
- Will use a tool called Metasploit which is a exploitation framework and it does more than exploitation 
command : MSF console 

<h2> Smbclient</h2>
-It will try to connect to the file share that is out there aka anonymously access.
command : smbclient -L \\\\<IP addresss>\\ or smbclient -L \\<IP address>
where -L is used to list the files 
