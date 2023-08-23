>[!Note] :What should be our Methodlogy when we are seeing a Website :
>- Service Version Information
>- Backend Directory's
>- Looking for Source Code
>- Potential Vulnerability Scanning With Nikto
>- Will explore the port 443,80,139 

Will start *Burp Suite* and Foxy-Proxy
If we find a default page it's an automatic finding.

80/443 - 192.168.142.129 09:54 AM
Default webpage - Apache - PHP
Information Disclosure - 404 page
Information Disclosure - server headers disclosure version information.



*Nikto* is a web vulnerability scanner but if the company has good security (i.e. Firewall it will *block* your request but it's not the case most of time)
```
command : nikto -h http://<IP address>
```





