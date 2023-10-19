>[!question] : What is a OSI Model ?_?
>OSI (Open Systems Interconnection) Model is a conceptual framework that standardized the functions of a communication system into 7 distinct layers and used as a reference for understanding network communication and protocols.


**Mnemonic**
`"Please Do Not Throw Sausage Pizza Away" ` can help you to remember all the Layers.


Overview : 
1 Physical            | data cables , cat6 
2 Data               | Switching , Mac addresses 
3 Network         | IP addresses , routing 
4 Transport       | TCP/UDP 
5 Session          | session management 
6 Presentation  | WMV , JPEG , MOV  | 3-way handshake
7 Application    | HTTP , SMTP 

<h2>In Detail: </h2>
1. Layer 1 - Physical
   - Deals with physical components: data cables (e.g., Cat6).

2. Layer 2 - Data Link
   - Switching and MAC addresses.
   - Responsible for reliable data transfer between two devices on the same network.

3. Layer 3 - Network
   - IP addresses and routing.
   - Determines the best path for data packets to reach their destination across different networks.

4. Layer 4 - Transport
   - TCP/UDP.
   - Responsible for end-to-end communication and error-checking to ensure data delivery.

5. Layer 5 - Session
   - Involves session management.
   - Establishes, maintains, and terminates connections between applications.

6. Layer 6 - Presentation
   - Data presentation and formatting.
   - Handles different file formats like WMV, JPEG, and MOV.

7. Layer 7 - Application
   - Application-layer protocols like HTTP and SMTP.
   - Interacts directly with end-user applications.


>[!important] :People in CS field will use terms like
layer 2 instead of switch
layer 3 instead of router
