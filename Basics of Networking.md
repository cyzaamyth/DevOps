### **Basics of Networking**

1. **What is internet ?**
    - The web or network of cables which transfers data from one location to other within connected devices.
2. **How does internet work?**
    - **OSI (Open System Interconnection) Model** - This is how internet works theoretically. The OSI model is a conceptual framework for understating how data is transmitted across a network, and it consists of seven layers:
        - **Application Layer** - for chatting whatsapp. File Transfer, Mail services, Directory services
        - **Presentation Layer -** identification or presentable, also responsible for data encryption and formatting. Data encoding, Encryption, Compression
        - **Session Layer -** both are online, session is maintained between them. Dialog control, Synchronization
        - **Transport Layer -** data or information transfer, messages/chat in this scenario. TCP, UDP. Service  Point addressing, Segmentation and reassembly, Flow control, Error control
        - **Network Layer -** It acts as a medium. Routing, Congestion control, Billing
        - **Data Link Layer** **-** Framing, Physical addressing, Error control, Flow control, Access control
        - **Physical Layer -** Physical characteristics of interfaces and media, Representation of bits., Data rate, Synchronization of bits, Line, configuration (point-to-point or multi-point), Transmission Mode, Physical Topology
- **TCP/IP (Transmission Control Protocol/ Internet Protocol) Model** **-** This is how internet actually works practically.
    - **Application Layer** - Protocol is a set of rules which include protocols like HTTP, HTTPS, SMTP, FTP
    - **Transport Layer** - TCP, UDP. Where the transmission of data is done over the internet.
        - **TCP** - Ensures reliable, error-checked, and ordered delivery of data between devices.
        - **UDP** - This protocol works during live stream where packet loss may happen. We can consider regular call with other person where the voice breaks under this protocol and low latency.
    - **Internet Layer** - Internet protocol, where the IP addresses gets generated.
    - **Network Layer**
- **Protocol -** The protocol field defines which upper-layer protocol data are encapsulated in
datagram (TCP, UDP, ICMP etc.). Every **protocol** has port number allotted to access the specific service that is running.
- **SSH(Secure Shell/Secure Socket Shell) -** SSH is a protocol for safely accessing distant computers via command line interaction. It uses port number 22 by default.
    
    ![image.png](attachment:1561e567-6224-4a2d-91d5-3caa226b3c4a:f5ffdcf9-8938-49ac-8f6e-9df1e16f27e6.png)
    
- **SCP(Secure Copy Protocol) -** The safe Copy Protocol, abbreviated "SCP," aids in the safe transmission of computer data from a local to a remote host. It is comparable to the File Transfer Protocol "FTP," but it also includes protection and authentication. The SCP operates on Port 22, and some believe it is a hybrid of the BSD RCP and the SSH protocol.
    
    ![image.png](attachment:a93a033d-8ce2-45b5-a6bf-5f6ee34d644a:image.png)
    
- **Subnet** is the logically explanation which still has IPv4 addresses in use. That divides a large network into smaller, manageable segments to improve network performance, security, efficiency by reducing broadcast traffic.
    
    ![image.png](attachment:4e8eb8b6-8d48-4002-9bf7-22a61e758a06:image.png)
    
- **VPN (Virtual Private Network)** ensure secure and private communication by encrypting data transmission between the user’s device and the internet.
- **Datagram -** Packets in IP layer are called Datagrams. A Datagram is a variable length packet(up to 65,536 bytes) consisting of two parts : Header and Data. The header can be from 20 to 60 bytes and contains information essential to routing and delivery
- Whenever internet changes IP address changes.
- **IPv4** is 32 bit address and **IPv6** is 64 bit address.
- **The MAC (Media Access Control) address / BIA (Burned In Address)** identifies the devices at a hardware level to gain the access to the internet. The **MAC** address is the physical address that individually recognises each device on a network. To interact between two networked devices, we need two addresses: an IP address and a MAC identifier. It is given to each NIC (Network Interface Card) capable of connecting to the internet.
    - Types of MAC Address are - Unicast, Multicast and Broadcast
    
    ![image.png](attachment:6fb3a576-78e6-4314-952d-d790a4a3b21c:91328f8c-78be-4d0f-9183-89be73b05182.png)
    
- **Data Centre** is nothing but the combination of multiple server rooms.
- Terminal and browser based clients are there.
- **Server** is where your application is hosted. It can be any sever (VM, Cloud, Instance, Physical)
- A **Firewall** is a network security system that monitors and controls network traffic based on predefined security rules.
- **Router** connects multiple networks and direct data packets to their destination based on IP address.
    - **Types of Routing :**
        - **Static Routing -** Nonadaptive routing, also called static routing, uses manually configured paths set by an administrator. Packets follow these fixed routes without considering network conditions or topology.
        - **Dynamic Routing -** Dynamic routing, also called adaptive routing, uses protocols like RIP or OSPF to automatically calculate and adjust the best paths based on real-time network conditions, ensuring continuous delivery even if a route fails.
        - **Default Routing -** Default Routing forwards all unspecified traffic to a single predefined gateway, serving as a catch-all for networks with a single exit point or a common destination. The router only uses this path when no specific route to the destination exists in its table.
    
    ![image.png](attachment:24ecce1e-d4df-434b-80e0-191eff94350a:image.png)
    
- A **Switch** connects multiple devices within the same network and forwards data to the correct destination using MAC address.
- **DNS (Domain Name Server)** resolves human-readable domain names (eg. google.com) into IP address used by computers for communication.
    - Types of DNS -
        - **Recursive queries** are those that require a DNS server to reply with the desired resource record. If an entry cannot be located, an error notice must be displayed to the DNS client.
        - **Iterative queries** are those in which the DNS client requests an answer from numerous DNS servers until the best response is discovered, or until an error or timeout happens. If the DNS server cannot discover a match for the query, it will forward the request to a DNS server authorised for a lower level of the domain namespace. The DNS client then queries this reference address, and the procedure is repeated with additional DNS servers.
        - **Non-recursive** requests are those that are handled by a DNS resolver when the requested resource is accessible, either because the server is authoritative or because the resource is already in cache.
- **Dynamic Host Configuration Protocol (DHCP)** is a network administration protocol that assigns an IP address to any device or component on a network so that they can interact using IP (Internet Protocol). These settings are automated and managed collectively by DHCP. There is no need to explicitly give IP addresses to new devices. As a result, no user setup is required to join to a DHCP-based network.
    
    ![image.png](attachment:30860a23-5989-432e-9297-df547ddbca73:image.png)
    
- **Client URL (pronounced "curl")** is a command line utility that allows data to be exchanged between a device and a website via a terminal. A user provides a server URL (the place where they want to make a request) and the data they want to transmit to that server URL using this command line interface (CLI). The cURL function makes use of the client-side URL transfer tool libcURL. Many various transmission methods are supported by this software, including HTTPS, SMTP, and FTP. When making queries, you can also include cookies, establish proxies, and add login details
    - Listing more than one URL:
    curl -O http://url1.com/file1.html -O http://url2.com/file2.html
    - cURL -T [chosen-file] "ftp://[target-destination]”
    - cURL smtp://[smtp-sever] --mail-from [sender] --mail-rcpt \ [receiver] --
    upload-file [mail-content-file]
    - cURL: cURL "dict://dict.org/d:hello"
