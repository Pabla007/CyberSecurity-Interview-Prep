> [! question] : What is IP address ?_?
 IP also know as Internet Protocol is a set of rules for communication over the internet.

**How it works ?_?**
It just work's like postal address assigned to our House where 2 addresses are being combined (i.e. your address + area Pin-Code)


It is divided into 2 Parts:

Prefix: The Network address that identifies the Physical network to which the computer is connected to.(i.e. The Network address comprises all hosts which belong to a specific network.)

Suffix: The Host address that identifies the individual computer on the network.
(i.e. The host address is the unique address of a particular host in that network.)

There are 4 classes of Ip address:
A B C D and we normally use Class C in our house /24

There are some Class A addresses that are reserved and cannot be used.
127.0.0.0 to 127.255.255.255  

<h2>LoopBack Address</h2>
IP address "127.0.0.1" is called the Loop Back Address.

<h2>Wild-Card Address</h2>
0.0.0.0 is a default route or unspecified address and it is used for connection from outside network.
python3 -m http.server

> [! important] : Key-Points:
> - We have solved the issue of shortage of ipv4 with NAT (i.e Network Address Translation ) using private ip address. 10.0.0.0 172.16.0.0 192.168.0.0 
> - So with single Class C public ip adress we can use upto 254 devices (i.e number of hosts per network).
> - IP address are layer 3 protocols (i.e layer 3 is a router) as we are talking about routing here.

Command to check the IP address in Linux is :
```
ifconfig
ip a
```

