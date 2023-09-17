<h2> The Lab Requirements For Active Directory :</h2>
Kali Linux
Windows Server 2019
Windows 10 Enterprise : Punisher & Peter Parker  
Punisher is a local admin on both the machines

We are just trying to Mimic the environment and all the setting are just almost are defaults and see what kind of attacks we can perform on this.

We have a Windows Server and Connected 2 windows users to it. (i.e. The Punisher and Peter Parker)

- Fcastle is a local user but `administrator` in both the PC's where on the other hand 
- Pparker is just a local user which has not admin rights.
And the security of pparker is handled by the organization (i.e. we have turned it off) but it is not the case of fcastle.


                                                                                                192.168.205.137
                                                                                                 Windows Server
                                                                                                |                        |
                                                                                             fcastle               pparker
                                                                                            |                                   |
                                                                               192.168.205.138             192.168.205.141 



