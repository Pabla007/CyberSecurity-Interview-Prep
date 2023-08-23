>[!Note] :What should be our Methodlogy when we are seeing a Website :
>- Service Version Information
>- Backend Directory's
>- Looking for Source Code
>- Potential Vulnerability Scanning With Nikto
>- Will explore the port 443,80,139 

<h2> Burp Suite</h2>
Will start *Burp Suite* and Foxy-Proxy
It's PROOF of concept that burp suite is your friend when it comes to Web Testing.
- Always view the source code of the website to get any kind of information disclosure / Keys /  Password etc
- Will intercept the request (i.e. refresh the target page 192.168.14.128 in our case) and will send it to Repeater.
- Repeater will show as our RESPONSE in REAL time so we can modify our request.
- Another thing we can do it go in the target and set a scope and will close the intercept 


If we find a default page it's an automatic finding.
80/443
Default webpage - Apache - PHP
Information Disclosure - 404 page
Information Disclosure - server headers disclosure version information.


<h2> Nikto</h2>
*Nikto* is a web vulnerability scanner but if the company has good security (i.e. Firewall it will *block* your request but it's not the case most of time)
```
command : nikto -h http://<IP address>
```



<h2> Directory Bursting</h2>
Now will use the tool called `dirbuster` (i.e. simply brute force to get the directory)but you can also use `gobuster` or `dirb`
Personally Like to use ffuf is an acronym for “fuzz faster you fool!” and Gobuster

command: dirbuster&
And when the pop up opens we will write the this ip address : http://192.168.142.129:80/


Response code :
200 means ok
400 means error (i.e. 404 page not found)
300 means redirect
500 means server error
 