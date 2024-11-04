- **Host-Only**: The VM will be assigned one IP, but it's only accessible by the box VM is running on. No other computers can access it.
    
- **NAT**: Just like your home network with a wireless router, the VM will be assigned in a separate subnet, like `192.168.6.1` is your host computer, and VM is `192.168.6.3`, then your VM can access outside network like your host, but no outside access to your VM directly, it's protected.
    
- **Bridged**: Your VM will be in the same network as your host, if your host IP is `172.16.120.45` then your VM will be like `172.16.120.50`. It can be accessed by all computers in your host network.

For a "Bridged" virtual network adapter, the host shares its physical adapters, i.e. the VM basically connects to the network like any other physical system. This also requires that the VM hat a valid IP address, or receive one from a DHCP server. With bridged networking, the VM is accessible from the network.

"NAT" on the other hand shares the hosts network connection by assigning the VMs an IP address from a private network, and translates network requests from the guest. This way the host appears as a single system to the network. VMs configured with NAT networking cannot be accessed from other systems on the network by default.

The reason why you cannot access the work network from the VM is likely caused by security policies, which prevent that unknown devices can access the network, or that only a single system can use a single network port.

