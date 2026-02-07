- **Basics of Networking**
1. What is internet ?
    - The web or network of cables which transfers data from one location to other within connected devices.
2. How does internet work?
    - **OSI (Open System Interconnection) Model** - This is how internet works theoretically.
        - Application Layer - for chatting whatsapp.
        - Presentation Layer - identification or presentable, also responsible for data encryption and formatting.
        - Session Layer - both are online, session is maintained between them
        - Transport Layer - data or information transfer, messages/chat in this scenario. TCP, UDP
        
        Hardware needed for all three following layers:
        
        - Network Layer - It acts as a medium.
        
        - Data Link Layer - to communicate both should have this. Cables and routers
        
        - Physical Layer - devices such as cables, mobiles, etc.
- **TCP/IP Model** - This is how internet actually works practically.
    - **Application Layer** - Protocol is a set of rules which include protocols like HTTP, HTTPS, SMTP, FTP
    - **Transport Layer** - TCP, UDP. Where the transmission of data is done over the internet.
        - **TCP** - Ensures reliable, error-checked, and ordered delivery of data between devices.
        - **UDP** - This protocol works during live stream where packet loss may happen. We can consider regular call with other person where the voice breaks under this protocol and low latency.
    - **Internet Layer** - Internet protocol, where the IP addresses gets generated.
    - **Network Layer**
- Every **protocol** has port number allotted to access the specific service that is running.
- **Subnet** is the logically explanation which still has IPv4 addresses in use. That divides a large network into smaller, manageable segments to improve network performance, security, efficiency by reducing broadcast traffic.
- **Virtual Private Network (VPN)** ensure secure and private communication by encrypting data transmission between the user’s device and the internet.
- Whenever internet changes IP address changes.
- **IPv4** is 32 bit address and **IPv6** is 64 bit address.
- **MAC** address identifies the devices at a hardware level to gain the access to the internet.
- **Data Centre** is nothing but the combination of multiple server rooms.
- Terminal and browser based clients are there.
- **Server** is where your application is hosted. It can be any sever (VM, Cloud, Instance, Physical)
- A **Firewall** is a network security system that monitors and controls network traffic based on predefined security rules.
- **Router** connects multiple networks and direct data packets to their destination based on IP address.
- A **Switch** connects multiple devices within the same network and forwards data to the correct destination using MAC address.
- **DNS (Domain Name Server)** resolves human-readable domain names (eg. google.com) into IP address used by computers for communication.
