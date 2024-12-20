# 1. Introduction to Networking

## 1.1 Introduction to Networks
    What is a Computer Network?
    The connection between two or more than two devices, nodes or points whether the link is wired or wireless
    is known to be a Network.


    Prior to Networking
    - Initial computer systems were Standalone devices.
    - All the resources would be directly connected to each devices.
    - The main resources that were used by the initial PC’s were Printers, Storage (Hard Drives), Scanners etc.
    - This led to loss of productivity in the company.
    - If a user had to print a document, he would need to copy the file to a removable media (Floppy Disks), move to the
      PC that was connected to the Printer, open the file from the Floppy and print it.
    - This is where network helped by connecting the devices (Computers, Printers etc.) to each other so that these
      resources could be shared with each other.


    Node - Any device which can share or receive the data is called a Node. 
    Channel - Through which the information or data propagate is known as channels, It can be guided(wired) or unguided
              (wireless).
    
    Goal of Networking
    - Shared hardware such as printers and input devices
    - Shared data and information through the use of shared storage devices
    - Communications such as email, instant messaging, chat rooms, etc.
    - Shared software, which is achieved by running applications on remote computers (Google GSuites, Microsoft office
    365, Dropbox, GMail)

    wired Network - Cables consist of Coaxial, UTP, STP, Fibre Optics . Centralized devices will be Switch or Hub.
                    Nowadays, Switch is preferred.
   
    Wireless Network - Radio waves or frequency. It uses Wireless Access Point device (equivalent to Switch in
                       wireless networking).

    Hybrid Network - uses both wired and wireless devices. The Wireless Access Point Connects to the Switch using
                     a Cable. The access point acts as a connection bridge between a wired and a wireless network.

    NIC - network interface card. Wi-Fi connections use wireless NICs (WLAN). Ethernet is the most popular wired
          LAN technology.
    RG-58 - Coaxial Cable connectore. BNC connector for RG58 cable. (Bayonet Neil-Concelman, or sometimes British
            Naval Connector) connector 
    RJ-45 - Registered Jack 45.
    T-connector - Tee Connector. used to split radio frequency power from a cable into two

    HUB -
    Switch -
    

![Untitled Diagram drawio](https://github.com/user-attachments/assets/6fa8684f-3fcf-43a8-9a53-1aea5cc05a32)

## 1.2 Network Types
    PAN - Personal Area Network
          This is the smallest and most basic type of network. A PAN is made up of a wireless AP, a computer/
          laptop or two, phones, printers, tablets, etc., and revolves around one person/family. These types of 
          networks are typically found in homes.
![Screenshot (687)](https://github.com/user-attachments/assets/581c6190-609b-4d79-86d0-9c9fb6010eb6)

    LAN -  Local Area Network
           LANs connect groups of nodes together across short distances. 
           LANs are networks that are either within a single building or between a group of 2 or 3 building close
           to each other. 
           LANs are one of the original types of networks. 
           The device that connects the networks to each other is called a Router.
![Screenshot (688)](https://github.com/user-attachments/assets/7cfaa092-dea1-46d8-8907-0d64583eae9d)

    MAN - Metropolitan Area Network
          A MAN is a computer network that usually covers a larger area than a LAN. 
          LAN covers a network in a single building or multiple buildings that are close to each other whereas
          a MAN spans a city.
          A MAN requires a Service Provider to connect the sites to each other.
          A MAN will connect the LAN’s to each other using a Router.
![Screenshot (689)](https://github.com/user-attachments/assets/2abe979b-3398-4ec3-bfa4-4f7b96ac0240)

    WAN (Private) - Wide Area Network
                    A WAN is a network that covers a large geographical area. 
                    A WAN may be spread across cities, countries or continents. 
                    When you connect LANs & MANs of the same company to each other, it is known as a Private
                    WAN.
                    You require the services of the Service Provider (SP) to connect the sites to each other.
![Screenshot (690)](https://github.com/user-attachments/assets/6acde9c9-23b4-4df3-a6bb-ea50daf91a2d)


    
    WAN (Public) Internet - The Internet is also an example of a WAN. But it is a WAN that connects LANs of 
                            different companies to each other, hence it is considered to be a Public WAN.
                            It allows the Company to publish and market its services to the general public. 
                            The Individual Users are also connected to the same network.
                            The Service Providers that allow a company or individual to connect to this “Network
                            of Networks” is known as a ISP (Internet Service Provider).
                            As you are connecting different networks to each other, they need to use the same 
                            language to communicate to each other. 
                            This communication protocol is called the Internet Protocol (IP).

    
![Screenshot (691)](https://github.com/user-attachments/assets/fd38c58d-8f7d-46a3-9e62-7922e3c60ec3)

    Switch - Connects devices in the same network.
    Router - Connects devices of different network.

## 1.3 Network Devices

    1. Hub -  It works on OSI Layer 1.A hub is a basically multi-port repeater. Hubs cannot filter data, so data
              packets are sent to all connected devices. In other words, the collision domain of all hosts
              connected through Hub remains one Hub. It is an unintelligent device that forwards the signal to
              all other ports and received by all connected devices, as a result all devices gets the unnecessary
              network traffic and causes network bandwidth problems.  

![Screenshot (684)](https://github.com/user-attachments/assets/e66f11f0-8a2c-4e28-a1f5-9a96a65c892e)

    
    2. Repeater - Operates at OSI Layer 1 i.e. Physical Layer. It just amplifies (or regenerate) the signal within
                  a same network before the signals become too weak or corrupted to to extend the length to which
                  the signal can be transmitted over the same network. When the signal becomes weak, they copy it
                  bit by bit and regenerate it at its star topology connectors connecting following the original
                  strength.
![IMG-20230828-WA0013](https://github.com/user-attachments/assets/105cf631-39e8-4098-b023-78ed5e6ebba9)

    
    3. Bridge - A bridge operates at the OSI Layer 2 i.e. Data Link Layer. A bridge is a repeater, with add on the
                functionality of filtering content by reading the MAC addresses of the source and destination. It
                is also used for interconnecting two LANs working on the same protocol.

![maxresdefault](https://github.com/user-attachments/assets/df36591f-7f39-41f6-a4b2-1446d04c5836)

    
    4. Switch (Layer 2 or Layer 3) - It works on OSI Layer 2 and uses MAC address(Media Access Control or Physical
                                     Address) of device to sends or forward the data to the another device to the
                                     destination device (destination device's MAC address) within a same network 
                                     typically (LAN). It is an intelligent device as compared to Hubs. A switch is
                                     a multiport bridge with a buffer and a design that can boost its efficiency(a
                                     large number of ports imply less traffic) and performance. The switch can 
                                     perform error checking before forwarding data, which makes it very efficient
                                     as it does not forward packets that have errors and forward good packets 
                                     selectively to the correct port only.  In other words, the
                                     switch divides the collision domain of hosts, but the broadcast domain remains
                                     the same.
![Screenshot (685)](https://github.com/user-attachments/assets/ccc058c8-9bca-489b-bbad-549fbba5dc19)

       Managed - Managed Switch have lots of option depending upon switch.
                 It has better security. We can segment our network into different VLAN, with some ports on one VLAN
                 and other ports on different VLAN. For example - put IoT devices into one VLAN and PCs into other
                 VLANs segment each other so that they can't communicate with each other.
                
       Unmangaed Switch - These are lot cheaper than managed switches. It comes with very limited features that are
                          only provided by Venodrs. In this, we can't change the configuration of the device. These
                          are plug and play, gives ability to extend the network. For example - if you plug ethernet
                          cable to unmanaged switch port then you can connect more devices to the network.
       
       Layer 3 Switch - This switch can be used in routing and therefore, operates at OSI layer 3. It supports VLAN
                        (Virtual Local Area Network), VLAN is a Subnet and it routes the traffic from one subnet to
                        another without a need of router locally.
    
    5. Modem - Modem stands for Modualtion and demodulation (analog to digital and digital to analog). A modem brings
               internet service into the home from internet service providers (ISPs). Some ISPs offer a combination of
               modem-router unit, known as a gateway.



               Most ISPs will either rent you a modem or sell you one outright. Many modems nowadays are "all-in-one"
               devices that also include a router, although you can still purchase a modem and router separately.

               There are three common types of modem connections:

               Dial-up — A modem that uses a phone line to connect to an ISP. This is the oldest type of modem
                         connection and has largely been replaced by broadband connections.
               
               DSL — A digital subscriber line modem uses a phone line to connect to an ISP but with much higher
                     speeds than dial-up.
               
               Cable — A modem that uses a cable TV line to connect to an ISP. This is the most common type of
                       modem connection.

![Modembak](https://github.com/user-attachments/assets/c9943c24-bec3-406f-b386-0a94059864f3)

    
    6. Router - Works on OSI Layer 3 and routes the data from one network to other using IP address (Source and
                Destination). TP-Link router, has LAN ports(basically switch port). routes the traffic from LAN
                to WAN. CISCO router, have switch ports and can act as a switch within LAN.
![download](https://github.com/user-attachments/assets/f1f4b0ff-a6ad-4983-9cdb-4d4c2aa3e974)
![router](https://github.com/user-attachments/assets/31a42e89-286b-4c1c-a7a9-5bea8c7f7249)

    
    7. Gateway -  A gateway, as the name suggests, is a passage to connect two networks that may work upon 
                  different networking models. They work as messenger agents that take data from one system,
                  interpret it, and transfer it to another system. Gateways are also called protocol converters
                  and can operate at any network layer. Gateways are generally more complex than switches or 
                  routers.
![img4](https://github.com/user-attachments/assets/87634ff9-8952-410f-abdf-a48ea23a6e10)

![Screenshot (686)](https://github.com/user-attachments/assets/86da2144-d73c-467d-a9de-618925137bc3)


    8. Brouter -  It is also known as the bridging router is a device that combines features of both bridge and 
                  router. It can work either at the data link layer or a network layer. Working as a router, it
                  is capable of routing packets across networks and working as the bridge, it is capable of 
                  filtering local area network traffic.

![download (1)](https://github.com/user-attachments/assets/12628f5b-caf3-4ddf-84ed-aad529b3fd3e)


    9. NIC - NIC or network interface card is a network adapter that is used to connect the computer to the 
             network. It is installed in the computer to establish a LAN.  It has a unique id that is written
             on the chip, and it has a connector to connect the cable to it. The cable acts as an interface 
             between the computer and the router or modem. NIC card is a layer 2 device which means that it
             works on both the physical and data link layers of the network model.

![download (2)](https://github.com/user-attachments/assets/ad4019d4-6b2a-443d-ade2-3abf7140f7d0)

![sddefault](https://github.com/user-attachments/assets/23035d6d-ac21-4d78-9b1a-e3175ffeeba9)




    Devices based on OSI layers

    Layer 7 : Application Layer
            Devices:
            
    Layer 6 : Presentation Layer
            Devices:
    
    Layer 5 : Session Layer
            Devices:
    
    Layer 4 : Transport Layer
            Devices:
            Firewall
    
    Layer 3 : Network Layer
            Devices:
            Routers
            Firewalls
            Layer 3 Switches
            VPN devices
    
    Layer 2 : Data Link Layer
            Devices:
            Ethernet Switches
            Bridges
            Wireless Access Points(WAPs)
            NICs
   
    Layer 1 : Physical Layer
            Devices:
            Cables (e.g., Co-axial cable, Fiber Optic, Ethernet cables(Generally UTP, STP))
            Hubs
            Repeaters
            NICs(Network Interface Card)
    
## 1.4 Network Topology
![Screenshot (694)](https://github.com/user-attachments/assets/61227703-4f6a-47ad-a95e-7106424eb12d)


    Network topology refers to how devices in a computer network are connected. Network Topology is the way that
    defines the structure, and how these components are connected. Network Topology is divided into two types:
    
    Physical Topology - refers to the actual arrangement of devices and cables in a network. It's how devices are
    physically connected to each other.
    
    Logical Topology - refers to the way data flows through a network, independent of the physical connections. It's
    how devices communicate with each other.

    In essence, while physical topology dictates the physical arrangement of devices, logical topology determines
    how data is transmitted and received within the network.


    Basic Terminology Related to Network Topology
    Node: A node refers to any device or point in the network, such as computers , servers , routers , or switches .
    These nodes are crucial for transmitting and receiving data within the network.
    Link: A link signifies a physical or logical connection between two nodes, allowing data to flow between them.
    Links can be wired (Ethernet cables) or wireless (Wi-Fi).
    Topology: Topology is the arrangement or layout of nodes and links in a network. It determines how devices are
    interconnected and how data travels within the network.
    
    Star - A central node(hub or switch) connects all devices.
           Data is transmitted from the central hub to each device.

           EX - A small office might use a node(Switches or Routers) as a central hub to connect computers, printers,
           and other devices.

    
    Bus - Devices are connected to a single cable.
          Data is transmitted from one device to another along the cable.

          Ex - Older Ethernet networks used bus topology, but it's less common today.
    
    Ring - Devices are connected in a closed loop.
           Data is transmitted in a circular fashion, from one device to the next.

           Ex - Token Ring networks were once popular but are now less common.

    
    Tree - A hierarchical structure where devices are connected to a central hub, which is then connected to
           other hubs.
           Similar to a star topology, but with multiple levels.

           Ex - Campus networks often use a tree topology to connect multiple buildings and departments.

    
    Mesh - Every device is connected to every other device.
           Provides high redundancy and fault tolerance.

           Ex - Large organizations might use a mesh topology for critical network segments to ensure high
                availability and redundancy.

    
    Hybrid - Combines two or more topologies.
             Offers flexibility and can be tailored to specific needs.

             Ex - Many corporate networks use a hybrid topology, combining star, bus, and ring topologies to
                  achieve optimal performance and reliability.
    Choosing the Right Topology - 
    The choice of topology depends on various factors, including:
    
    Network size and complexity: Smaller networks may benefit from simpler topologies like star or bus, while
                                 larger networks might require more complex topologies like mesh or hybrid.
    Performance requirements: High-performance networks may require topologies that minimize latency and maximize
                              bandwidth, such as mesh or hybrid.
    Reliability and fault tolerance: Redundant topologies like mesh can improve reliability and fault tolerance.
    Cost: Some topologies, like mesh, can be more expensive to implement due to the number of cables and devices
    required.
    By understanding these topologies and their characteristics, organizations can design and implement networks that
    meet their specific needs.

## 1.5 TCP/IP vs OSI Layer

    OSI Layer - The OSI reference model was developed by ISO – ‘International Organization for Standardization ‘,
                in the year 1984.The OSI model, created in 1984 by ISO , is a reference framework that explains 
                the process of transmitting data between computers. OSI stands for Open Systems Interconnection ,
                where open stands to say non-proprietary. All these 7 layers work collaboratively to transmit the 
                data from one person to another across the globe.

                The OSI model provides a theoretical foundation for understanding network communication.

    
    Application Layer: Applications create the data.
    Presentation Layer: Data is formatted and encrypted.
    Session Layer: Connections are established and managed.
    Transport Layer: Data is broken into segments for reliable delivery.
    Network Layer : Segments are packaged into packets and routed.
    Data Link Layer: Packets are framed and sent to the next device.
    Physical Layer: Frames are converted into bits and transmitted physically.

    Each layer adds specific information to ensure the data reaches its destination correctly, and these steps
    are reversed upon arrival.

![cn1](https://github.com/user-attachments/assets/8ed293f9-8e94-42ef-81fd-d8a726150318)

    Example Scenarios - 

    Alex sends an e-mail to his friend David.

    Step 1: Alex interacts with e-mail application like Gmail , outlook , etc. Writes his email to send. (This
            happens in Layer 7: Application layer )
            
    Step 2: Mail application prepares for data transmission like encrypting data and formatting it for transmission.
            (This happens in Layer 6: Presentation Layer )
    
    Step 3: There is a connection established between the sender and receiver on the internet. (This happens in 
            Layer 5: Session Layer )
    
    Step 4: Email data is broken into smaller segments. It adds sequence number and error-checking information to
            maintain the reliability of the information. (This happens in Layer 4: Transport Layer )
    
    Step 5: Addressing of packets is done in order to find the best route for transfer. (This happens in Layer 3:
            Network Layer )
    
    Step 6: Data packets are encapsulated into frames, then MAC address is added for local devices and then it 
            checks for error using error detection. (This happens in Layer 2: Data Link Layer )
    
    Step 7: Lastly Frames are transmitted in the form of electrical/ optical signals over a physical network 
            medium like ethernet cable or WiFi.
    
    After the email reaches the receiver i.e. David, the process will reverse and decrypt the e-mail content. At
    last, the email will be shown on David’s email client.

    
    Layer 7: Application layer 
    
             Function - The Application Layer (Layer 7) is the topmost layer of the OSI model and provides the
                        interface between the network services and end-user applications. This layer enables 
                        end-users to interact with software applications for data exchange and communication 
                        over the network, and it directly supports services such as email, file transfer, and
                        web browsing.

                        Resource Sharing: Provides a platform for sharing network resources like files, printers,
                        or databases.
                       
                       Remote Access: Allows users to access applications on remote systems.
                       
                       File and Data Transfer: Facilitates secure and organized data transfers between devices.
                       
                       Email and Messaging: Manages the transfer and storage of messages through email protocols.
                       
                       For example, when a user logs into a website, the Application Layer processes the login
                       request, uses an HTTP or HTTPS connection, and returns the requested page to the user.
                        
             Devices - Devices associated with the Application Layer include:

                       Web Servers: Handle HTTP and HTTPS requests for web services.
                       Email Servers: Manage email traffic using SMTP, IMAP, or POP protocols.
                       DNS Servers: Translate domain names into IP addresses, enabling web browsing.
                       File Servers: Manage file access and transfers within a network.

             
             Secure protocol - HTTPS (HyperText Transfer Protocol Secure): Encrypts web traffic, securing
                               communication between users and web servers. Widely used for secure web browsing.
                               
                              FTPS and SFTP (Secure File Transfer Protocol): Secure methods for transferring files,
                              with encryption for data protection.
                              
                              SMTPS (Simple Mail Transfer Protocol Secure): Secures email communication by adding
                              encryption and authentication.

             
             unsecure protocol - HTTP (HyperText Transfer Protocol): Transfers web content without encryption, 
                                 making it vulnerable to interception.
                                 FTP (File Transfer Protocol): Transfers files without encryption, exposing file
                                 contents and user credentials to attackers.
                                 
                                 SMTP (Simple Mail Transfer Protocol): Transmits emails without encryption,
                                 allowing potential access to message content if intercepted.

             
             
             Attack scenario - A common attack at the Application Layer is the Phishing Attack:

                               Phishing Attack Scenario: Phishing attacks use fraudulent messages or websites
                               to deceive users into disclosing sensitive information such as passwords or credit
                               card details. Attackers often impersonate legitimate services (e.g., a bank) to trick users.
                               
                               Example: An attacker sends an email posing as a financial institution, urging the user to log
                               in and verify their account details. When the user clicks the link, they are directed to a fake
                               site that captures their credentials.

             
             prevention mechanism - Email Filtering and Anti-Phishing Software: Scans and filters out suspicious
                                    emails to protect users from phishing.
                                    
                                    Multi-Factor Authentication (MFA): Adds additional verification steps, making
                                    it difficult for attackers to access accounts even if they obtain login credentials.
                                    
                                    User Education and Awareness: Educating users about phishing tactics helps them
                                    recognize and avoid fraudulent websites or emails.
             
             Defense against attack - SSL/TLS Certificates: Ensure that websites are legitimate and provide encryption,
                                      helping users verify the authenticity of websites.
                                      
                                      DNS Security Extensions (DNSSEC): Protects DNS responses from being tampered
                                      with, reducing the risk of phishing and DNS spoofing.
                                      
                                      Regular Security Audits: Helps identify potential vulnerabilities in web
                                      applications and closes security gaps.
    
    Layer 6: Presentation layer
    
             Function - The Presentation Layer (Layer 6) is responsible for data formatting, translation, 
                        encryption, and compression, ensuring that data is presented to the Application Layer
                        in a readable format for both the sender and receiver. It essentially acts as a translator
                        and encoder/decoder between the data generated by the application and the data transmitted
                        over the network.

                        Data Translation: Converts data between various formats such as ASCII, EBCDIC, or different
                        image, audio, and video formats.
                        
                        Data Encryption and Decryption: Secures data by encrypting it before transmission and
                        decrypting it at the destination.
                        
                        Data Compression and Decompression: Reduces data size for efficient transmission and 
                        decompresses data on the receiving end for use.
                        Character Encoding: Transforms data into standardized character sets like UTF-8 or ASCII.
                        
                        For example, when a user uploads an image file, the Presentation Layer may compress the file
                        before sending it across the network and then decompress it on the receiver’s end.

             
             Devices -  The Presentation Layer doesn’t involve specific hardware but includes:

                        Encryption and Decryption Gateways: Secure servers or software components responsible
                        for encrypting/decrypting data before it passes through the network.
                        
                        Data Format Converters: Software that translates file formats, such as media codecs for
                        audio and video streaming.
                        
                        Compression and Decompression Software: Used in multimedia applications where data needs
                        to be compressed (like JPEG or MP3 codecs).
             
             Secure protocol - SSL/TLS (Secure Sockets Layer / Transport Layer Security): While SSL/TLS operates
                               primarily between the Presentation and Transport layers, it is responsible for 
                               encrypting and decrypting data at the Presentation Layer. TLS secures data 
                               transmitted between web browsers and servers (HTTPS).
                               
                               MIME (Multipurpose Internet Mail Extensions): MIME is a standard for encoding 
                               multimedia data in emails, allowing attachments to be securely and efficiently transmitted.
             
             unsecure protocol - Telnet (Unencrypted Text Transfer): Telnet is an example of an unencrypted protocol
                                 at this layer. It transmits data in plaintext, making it vulnerable to interception.
                                 
                                 FTP (File Transfer Protocol): FTP transmits files in plaintext without encryption,
                                 exposing data during file transfers to potential attackers.
             
             Attack scenario - A common attack at the Presentation Layer is Man-in-the-Middle (MITM) Attacks that
                               target unencrypted data:

                               MITM Attack Scenario: In an MITM attack, an attacker intercepts data being transmitted
                               between two devices. If encryption is not in place, the attacker can read, modify, or
                               inject malicious data into the communication.
                               
                               Example: A user logs into an email account over HTTP (unencrypted) in a public network.
                               An attacker intercepts the login credentials and gains unauthorized access.

             
             prevention mechanism - Use of Strong Encryption Protocols (SSL/TLS): Encrypts data to prevent 
                                    interception and ensures that only authorized parties can read the data.
                                    
                                    Digital Certificates and Public Key Infrastructure (PKI): Verifies the 
                                    authenticity of devices and prevents attackers from impersonating legitimate users.
                                    
                                    Encoding Standards: By ensuring consistent character encoding (e.g., UTF-8), the 
                                    Presentation Layer prevents misinterpretations or alterations that attackers might exploit.
             
             Defense against attack - TLS Encryption: Encrypts data to prevent eavesdropping and tampering, 
                                      ensuring secure data presentation and transmission.
                                      
                                      Use of HTTPS: Enforces encrypted communication between clients and servers
                                      to protect against MITM attacks.
                                      
                                      Intrusion Detection Systems (IDS): Monitors for suspicious activities and
                                      alerts administrators to potential MITM attacks or data tampering attempts.
    
    Layer 5: Session layer ()
    
             Function - The Session Layer (Layer 5) is responsible for establishing, maintaining, and 
                        terminating communication sessions between applications on different devices. 
                        It manages and controls the dialogue between computers by setting up, coordinating,
                        and ending interactions, making it possible for devices to exchange data efficiently
                        in a synchronized way.

                        Session Establishment, Maintenance, and Termination: Manages the start, continuation,
                        and end of communication sessions between devices.
                        
                        Synchronization: Adds checkpoints in data streams to help resume communication smoothly
                        in case of interruptions.
                        Dialog Control: Controls the mode of communication, determining whether it is 
                        half-duplex (one-way at a time) or full-duplex (two-way simultaneously).
                        
                        Session Recovery: Manages reconnection and data recovery processes if there is an 
                        unexpected interruption in communication.
                        This layer is especially important in applications where continuous, long-running data 
                        transfers or multimedia sessions are common, such as in video calls and streaming.

             
             Devices - While the Session Layer does not involve specific hardware devices (like routers or switches),
                       some software components work at this layer:

                       Application Servers: Hosts for applications that need to maintain sessions, such as video
                       conferencing and file transfer servers.
                       
                       Middleware: Components like session brokers or session managers in distributed computing
                       environments handle sessions between clients and servers.

             
             Secure protocol - NetBIOS over TCP/IP (NBT) with Security Extensions: Helps with the establishment 
                               of session-level connections between devices in Windows networks, allowing for 
                               secure communication and access control.
                               
                               RPC (Remote Procedure Call) over TLS: Allows remote execution of functions over 
                               a network securely by encrypting the session data, ensuring that only authenticated
                               and authorized calls are processed.
             
             unsecure protocol - NetBIOS (Network Basic Input/Output System): Without encryption or authentication,
                                 NetBIOS can be exploited by attackers to access shared resources within a network.
                                 
                                 RPC without TLS: Transmits remote procedure calls in cleartext, making it vulnerable
                                 to interception and misuse by attackers.

             
             Attack scenario - Session Hijacking Attack: In this attack, an attacker takes control of an ongoing
                               session between two devices. By capturing session tokens or session IDs, an 
                               attacker can impersonate a legitimate user and gain unauthorized access to resources.
                               
                               Example: During a video conference session, an attacker intercepts the session 
                               token and replays it, allowing them to join the session without authorization, 
                               potentially gaining access to confidential discussions.
             
             prevention mechanism - Session Timeout and Re-authentication: Sets an expiration for session tokens,
                                    requiring users to re-authenticate if they remain inactive, reducing the 
                                    window of opportunity for an attacker.
                                    
                                    Token Encryption and Validation: Encrypts session tokens and validates them
                                    on the server side, ensuring only authorized users can use valid tokens.
                                    
                                    Multi-Factor Authentication (MFA): Adds additional authentication steps 
                                    during session establishment to prevent attackers from hijacking sessions.
             
             Defense against attack - Secure Protocols (e.g., TLS): Encrypts session data to prevent interception
                                      and modification by attackers.
                                      Token Rotation and Validation: Regularly updates session tokens and verifies
                                      their legitimacy, making it harder for attackers to use stolen tokens.
                                      
                                      Intrusion Detection and Prevention Systems (IDPS): Monitors session behavior
                                      and detects anomalies, such as unexpected replays or session takeovers.
    
    Layer 4: Transport layer (Data = Segments)
    
             Function - The Transport Layer (Layer 4) is responsible for reliable data transfer between devices
                        by managing data segmentation, flow control, error handling, and ensuring data integrity.
                        It establishes, maintains, and terminates connections between sender and receiver, making
                        sure that data reaches its destination correctly and in sequence.

                        Segmentation and Reassembly: Breaks large data packets into smaller segments and 
                        reassembles them on the receiving end.
                        Connection Establishment and Termination: Sets up and tears down connections 
                        between applications.
                        Flow Control: Manages data transmission rates to prevent network congestion and 
                        ensure efficient transfer.
                        Error Detection and Correction: Detects transmission errors and requests retransmission
                        if necessary to maintain data integrity.
                        
                        For example, when downloading a large file, the Transport Layer segments the file into
                        smaller packets, sends them in sequence, and reassembles them at the destination.



             Devices - Firewall Appliances: Can operate at the Transport Layer to block or allow specific port
                       numbers or protocols.
                       
                       Network Address Translators (NAT): Often involved in managing port numbers and 
                       connections for multiple devices.
                       
                       Load Balancers: Operate at the Transport Layer to distribute network traffic across 
                       multiple servers for scalability and redundancy.
                       
             Secure protocol - TLS (Transport Layer Security): Encrypts data at the Transport Layer to protect it
                               during transmission and prevent eavesdropping or tampering.
                               
                               DTLS (Datagram Transport Layer Security): A variant of TLS designed for 
                               datagram-based protocols (like UDP), commonly used in VoIP or online gaming for 
                               secure, real-time data transmission.

             
             unsecure protocol - TCP (Transmission Control Protocol): Manages connections and guarantees data
                                 delivery but does not inherently encrypt data, making it susceptible to interception.
                                 
                                 UDP (User Datagram Protocol): Provides fast but connectionless and unencrypted
                                 data transmission. Used in real-time applications like online gaming and streaming,
                                 which are sensitive to latency but prioritize speed over security.

             Attack scenario - TCP SYN Flood Attack Scenario: In this attack, the attacker initiates multiple 
                               TCP connection requests to a server without completing the handshake process. 
                               The server allocates resources to each incomplete connection, eventually 
                               overwhelming the server and preventing legitimate users from accessing it.
                               
                               Example: An attacker sends numerous SYN packets to a web server. Since the attacker
                               never completes the handshake, the server's resources are drained as it waits for 
                               completion, causing service disruption.
             
             prevention mechanism - SYN Cookies: A method to handle initial SYN packets without allocating 
                                    resources immediately, allowing the server to verify the connection request
                                    before committing resources.
                                    
                                    Rate Limiting: Controls the number of incoming requests over a specified 
                                    period to prevent overwhelming the server.
                                    
                                    Firewall Rules: Firewalls can be configured to block suspicious IP addresses
                                    or limit connection attempts to prevent abuse.
             
             Defense against attack - Intrusion Prevention Systems (IPS): Monitors network traffic in real-time
                                      to detect and respond to SYN floods or other Transport Layer attacks.
                                      
                                      Load Balancers: Distribute incoming requests across multiple servers, making
                                      it harder for attackers to overwhelm a single server with SYN floods.
                                      
                                      TCP RST Packets: Sends reset packets to close half-open connections and free
                                      up server resources.


    
    Layer 3: Network layer (Data = Packets)
             Function - The Network Layer (Layer 3) is responsible for the routing, forwarding, and addressing 
                        of data packets across multiple interconnected networks. It provides mechanisms for 
                        packet switching, logical addressing, and routing so that data can travel across various
                        paths in an internetworked environment to reach its destination.

                        Routing: Determines the best path for data packets to travel from source to destination
                        across networks.
                        
                        Logical Addressing: Uses IP addresses to uniquely identify each device on a network, 
                        allowing packets to find their intended destination.
                        
                        Fragmentation and Reassembly: If data packets are too large for the transmission medium,
                        the Network Layer fragments them and reassembles them at the destination.
                        
                        Packet Forwarding: Moves packets through routers along the network path.

             Devices - Routers and layer 3 Switch
             
             Secure protocol - IPsec (Internet Protocol Security): A suite of protocols that provides authentication,
                               integrity, and encryption for IP packets, often used in VPNs (Virtual Private Networks)
                               to secure data traveling across public or insecure networks.

             
             unsecure protocol - IPv4 (Internet Protocol version 4): While essential for addressing and routing, 
                                 IPv4 lacks inherent security mechanisms like encryption or authentication, making
                                 it vulnerable to various attacks, including spoofing and sniffing.
                                 
                                 ICMP (Internet Control Message Protocol): While useful for diagnostic tools 
                                 like ping, ICMP is often exploited for network reconnaissance and Denial of 
                                 Service (DoS) attacks.

                                 IPv6
             
             Attack scenario - IP Spoofing Attack: In IP spoofing, an attacker forges the source IP address of 
                               data packets, making them appear as though they come from a trusted source. This
                               can allow the attacker to bypass network security controls, impersonate trusted 
                               devices, or launch further attacks like Distributed Denial of Service (DDoS).
                               
                               Example: An attacker might send packets to a target server with a spoofed IP address
                               of a trusted device. The server, believing the packets are legitimate, responds and
                               potentially allows unauthorized access or redirects the attacker's traffic to a victim.
             
             prevention mechanism - Ingress and Egress Filtering: Network routers and firewalls can be configured to 
                                    filter incoming and outgoing traffic based on trusted IP addresses, preventing
                                    packets with suspicious or forged IP addresses from entering or exiting the network.
                                    
                                    Use of IPsec: Encrypting and authenticating IP packets with IPsec helps ensure
                                    that only authorized devices communicate, protecting against IP spoofing and
                                    similar attacks.
                                    Access Control Lists (ACLs): ACLs on routers or firewalls allow only specified
                                    IP addresses or ranges to communicate, blocking spoofed or unauthorized addresses.
             
             Defense against attack - Router Configuration and Network Monitoring: Configure routers to block 
                                      invalid or private IP addresses on public interfaces. Employ network 
                                      monitoring tools that detect and alert on anomalies in IP traffic.
                                      
                                      Packet Filtering Firewalls: Implement firewalls that inspect and filter 
                                      packets based on IP header information, helping to block malicious IP 
                                      addresses or suspicious patterns.
                                      Intrusion Detection and Prevention Systems (IDS/IPS): IDS/IPS tools monitor
                                      network traffic for patterns associated with IP spoofing or DDoS and can 
                                      automatically block or alert on such activities.


    
    Layer 2: Data link layer (Data = Frames)
    
             Function - The Data Link Layer (Layer 2) is responsible for the node-to-node transfer of data and
                        error detection and correction. It ensures that data frames are reliably transmitted 
                        between nodes on the same network or local area network (LAN) by managing how data 
                        packets are encoded, decoded, and transmitted over a physical medium.

                        Framing: Divides data into frames for easier handling and transmission.
                        Error Detection and Correction: Uses error-detection codes to identify and correct 
                        errors during transmission.
                        Flow Control: Ensures that data flows smoothly, preventing faster devices from 
                        overwhelming slower ones.
                        MAC Addressing: Assigns a unique Media Access Control (MAC) address to each device, 
                        enabling local addressing.
                        
                        The Data Link Layer is divided into two sublayers:

                        Logical Link Control (LLC): Responsible for flow control and error handling.
                        Media Access Control (MAC): Manages physical addressing and access to the transmission
                        medium.

             
             Devices - Switches, Bridges, NICs
             
             Secure protocol - 802.1X: A secure access control protocol that authenticates devices attempting to
                               connect to a LAN or WLAN. It helps prevent unauthorized devices from accessing 
                               network resources.

                               
             
             unsecure protocol - ARP is essential in IP networking to map IP addresses to MAC addresses. However,
                                 it lacks authentication and is vulnerable to ARP spoofing and ARP cache poisoning 
                                 attacks.
             
             Attack scenario - ARP Spoofing Attack: The attacker sends fake ARP messages to associate their MAC 
                               address with the IP address of another device (like a gateway or server). This 
                               allows the attacker to intercept, modify, or stop data destined for the 
                               legitimate device.
                               
                               Example: In a corporate LAN, an attacker could impersonate the network gateway by
                               spoofing its IP address, allowing the attacker to intercept data, alter its 
                               contents, or even perform a denial of service attack.
             
             prevention mechanism - Port Security: Configuring switch ports to only allow specific MAC addresses
                                    to connect, limiting unauthorized device access.
                                    Dynamic ARP Inspection (DAI): Verifies ARP requests and responses against a 
                                    trusted table of known IP-MAC pairs to prevent spoofing.
                                    Use of Virtual LANs (VLANs): Segments network traffic and limits access based
                                    on logical groupings, reducing the impact of potential attacks.

             
             Defense against attack - Implement 802.1X Authentication: Ensures only authenticated devices can 
                                      connect to the network, which helps prevent unauthorized access and 
                                      spoofing.
                                      Network Monitoring Tools: Use intrusion detection systems (IDS) and 
                                      intrusion prevention systems (IPS) to detect and mitigate anomalies in 
                                      network traffic.
                                      MAC Address Filtering: Allows only specified MAC addresses to communicate,
                                      reducing exposure to unauthorized devices.

    
    Layer 1: Physical layer(Data = Bits)
    
             Function - The Physical Layer is responsible for the actual physical connection between devices and
                        the transmission of raw binary data (bits) as electrical, optical, or radio signals.

                        Data Encoding and Signaling: Converting binary data to signals for transmission over the
                        medium.
                        Bit Synchronization: Ensuring sender and receiver are in sync for data interpretation.
                        Transmission Mode: simplex (one way), half-duplex (two-way, one direction at a time), and
                        full-duplex (two-way, simultaneous).
                        
             Devices - Hubs, Repeaters, NICs, Cables & Connectors (Ethernet Cat5 or Cat6), fiber optic cables,
                       and coaxial cables
             
             Secure protocol - Since this layer deals with the transmission medium, it doesn’t handle encryption
                               or security protocols at a data level. Physical security measures are implemented
                               instead.
             
             unsecure protocol - Ethernet (at the lowest layer): At the basic level, Ethernet cables and 
                                 infrastructure don't inherently include encryption, leaving them vulnerable to
                                 physical tapping or interception.

                                 Wi-Fi Signal Jamming through interference.
             Attack scenario - Wiretapping Attack: An attacker physically connects a device to a cable or 
                               intercepts wireless signals to capture data being transmitted. This is easier with
                               unshielded Ethernet cables or unsecured wireless connections.
                               
                               Example: In a data center, an attacker gains access to network cables and uses 
                               hardware to capture data transmitted through them, potentially stealing sensitive 
                               information like usernames, passwords, or proprietary data.
             
             prevention mechanism - Use Shielded Cables and Secure Enclosures: Shielded twisted-pair cables or
                                    fiber optic cables are harder to tap and protect against electromagnetic 
                                    interference.
                                    
                                    Physical Security Measures: Restrict physical access to networking equipment
                                    through locks, CCTV, secure data cabinets, and surveillance.
                                    Wireless Security Configurations: For wireless connections, use encryption 
                                    protocols like WPA3 to secure data transmitted over radio waves.
             
             Defense against attack - Regular Physical Security Audits: Conduct audits to ensure only authorized
                                      personnel can access networking hardware.
                                      Network Monitoring for Unusual Activity: Employ Intrusion Detection Systems
                                      (IDS) to monitor and alert on unusual data traffic patterns that might 
                                      indicate unauthorized data capturing. Tamper-Evident Seals and Locks: Use
                                      tamper-evident mechanisms on physical enclosures to detect if hardware or 
                                      cables have been accessed or altered.

> [!IMPORTANT]
> Network Layer, Data Link Layer, and Physical Layer are also known as  Lower Layers  or  Hardware Layers  .
> Session Layer, Presentation Layer and Application Layer are also known as  Upper Layers or  Software Layers. 
> The transport layer is called as  Heart of the OSI  model. 

https://www.geeksforgeeks.org/open-systems-interconnection-model-osi/
https://www.byos.io/blog/types-of-cyber-attacks-osi

    TCP/IP Layer -
    Layer 4: Application layer (application,presentation,session layer)
             Function
             Devices
             Secure protocol
             unsecure protocol
             Attack scenario
             prevention mechanism
             Defense against attack
    
    Layer 3: Transport layer
             Function
             Devices
             Secure protocol
             unsecure protocol
             Attack scenario
             prevention mechanism
             Defense against attack
    
    Layer 2: Internet or Network layer
             Function
             Devices
             Secure protocol
             unsecure protocol
             Attack scenario
             prevention mechanism
             Defense against attack
    
    Layer 1: Network Access layer(data link,physical layer)
             Function
             Devices
             Secure protocol
             unsecure protocol
             Attack scenario
             prevention mechanism
             Defense against attack

![Screenshot (630)](https://github.com/user-attachments/assets/2eaa585a-3cde-4704-b493-90fd706200a6)

## 1.6 The Internet & DNS
    The Internet - The “Internet” is a global system of interconnected computer networks that connects all the
                   individual networks to each other. 
                   These networks include the Government, Schools, Colleges, Universities, Private Businesses,
                   Individual people etc. It is also called the “Network of Networks”. 
                   It uses a common protocol [Language] to allow networks to communicate to each other. The 
                   protocol is called the Internet Protocol [IP]. 
                   Each device connected to the Internet is uniquely identified using an address known as the IP
                   Address. [200.1.1.5]. This unique IP Address is known as the Public Address of the device.
                   These addresses are controlled by an entity known as the Internet Address Numbers Authority (IANA).
                   IANA allocates the addresses to the ISPs. The ISPs are responsible for assigning the IP Addresses to
                   Companies and Individual users and making sure they are unique. 
                    
    
    Basics Services / Protocols on the Internet -
    
    Web Services(Web Server or WWW) - The most common service on the Internet. It is used to provide information to
                                      the End-Users. It uses a protocol called HTTP to allow a client using an 
                                      application called a browser to connect to the a Server that is running the Web Server.
    
    Email Service(SMTP) - Another common service on the Internet is the E-Mail services. It allows end-users and companies
                          to send mail messages to each other. It uses a protocol called SMTP to allow a client to send
                          E-mails.
    
    Name Services(DNS) - It allows devices to communicate to each other using Names rather than IP Addresses. It uses
                         a protocol called DNS to allow client to resolve the Name of a device to its corresponding 
                         address. This service is explained later in this module.
    Internet Connections
![Screenshot (692)](https://github.com/user-attachments/assets/a2331d75-7bcc-487d-b33b-a52b912faf44)

    DNS - Domain Name System
          When we want to access a server on the Internet like Facebook, Google etc., we need to know the Server’s
          IP Address.
          As humans, we are used to addressing entities using names not addresses. For example, if we want to go to
          a City, we will use the name of the city, not its Postal Code/Zip Code.
          But the Internet communications are based on Addresses. So a mechanism was designed to make it easier
          for users to access resources on the Internet. 
          The companies had to register a Domain Name in addition to acquiring an IP Address range from the ISP.
          The company would then assign the servers a name in addition to the unique IP Address.
          The users could refer to the server using its name rather than the IP Address.
          A server known as the Domain Name System (DNS) was designed to provide the resolution between the Name
          of the device to its IP Address.
         Each Domain would have its own DNS Server that would do the name resolution for that Domain/Company devices.
         The IP Address of the DNS / Name Server for the Domains is on the Root DNS Servers. 
![Screenshot (693)](https://github.com/user-attachments/assets/ffb0ecb0-52b0-4fa5-b7ad-eea4543bee1f)

    
    DNS Communication Process -
    Step 1 : User types www.khawarb.com.
    Step 2 : The User’s PC will send a DNS resolution request to it’s DNS server generally the ISP’s DNS Server
             (150.5.1.11), to find the IP Address for www.khawarb.com. 
    Step 3 : The ISP’s DNS Server will send a request to the Root DNS Server (50.5.5.5) to find the DNS for khawarb.com.
             The Root DNS Server will respond with 199.1.1.6, the DNS Server for khawarb.com.
    Step 4 : The ISP’s DNS now send a DNS resolution request to khawarb.com’s DNS server (199.1.1.6) asking for the IP
             address for www.khawarb.com.
    Step 5: The DNS Server for khawarb.com will respond back with the IP Address for www.khawarb.com (199.1.1.7).
    Step 6: The ISP DNS Server will receive the IP address and forward it to the User’s PC.
    Step 7: The User’s PC will use the 199.1.1.7 destination address to send the request.
    Note: The whole procedure is done within Seconds.

## 1.7 Network Ports
    In the world of computer networking, network ports are like virtual doors that allow different applications
    and services to communicate with each other. They serve as specific addresses within a computer or network 
    device, helping to direct incoming and outgoing data to the correct destinations.
    
    In cybersecurity, network ports are categorized as either secured or unsecured based on their use in secure
    protocols (such as those using encryption) or unsecured protocols (which transmit data in plaintext).


**Secured Ports**<br>
These are typically used by protocols that encrypt communications to ensure privacy and integrity.

|Ports|Protcols|Descriptions|
|----------|-------------|--|
|443|HTTPS|Secure web traffic using SSL/TLS encryption.|
|22|SSH|Secure Shell, for secure remote administration and file transfer.|
|465/587|SMTPS|Secure SMTP for sending encrypted emails.|
|993|IMAPS|Secure version of IMAP (Internet Message Access Protocol).|
|995|POP3S|Secure version of POP3 (Post Office Protocol).|
|3389|RDP|Remote Desktop Protocol for secure remote access (with encryption).|
|989/990|FTPS|Secure File Transfer Protocol over SSL/TLS.|
|636|LDAPS|Secure LDAP (Lightweight Directory Access Protocol) over SSL.|
|8443|HTTPS (alt)|Alternative port for HTTPS.|
|853|DNS over TLS|Secure DNS queries over TLS.|

**Unsecured Ports**<br>
These are used by protocols that transmit data in plaintext, making them more vulnerable to attacks like 
eavesdropping or man-in-the-middle attacks.

|Ports|Protcols|Descriptions|
|----------|-------------|--|
|80|HTTP|Unencrypted web traffic.|
|21|FTP|File Transfer Protocol, sends data and credentials in plaintext.|
|23|TELNET|Unencrypted remote login service.|
|25|SMTP|Unsecured Simple Mail Transfer Protocol.|
|110|POP3|Unsecured version of Post Office Protocol for retrieving emails.|
|143|IMAP|Unsecured Internet Message Access Protocol.|
|53|DNS|Domain Name System, vulnerable to DNS spoofing.|
|69|TFTP|Trivial File Transfer Protocol, no encryption or authentication.|
|8443|HTTPS (alt)|Alternative port for HTTPS.|
|445|SMB|Server Message Block, often a target for malware/worms.|
|139|NetBIOS|Network Basic Input/Output System, can be exploited for attacks.|
|161/162|SNMP|Simple Network Management Protocol, sends data without encryption.|
|2049|NFS|Network File System, lacks encryption by default.|
|123|NTP|Network Time Protocol, vulnerable to amplification attacks.|

# 1.8 Communication Medias

    Wired -Wired communication technologies use physical cables to transmit data between devices.
    
    Examples-
    Co-axial cable
    STP UTP - ( Shielded and Unshielded Twisted Pair)
    Fiber Optics
    
    Wireless - Wireless communication technologies use electromagnetic waves to transmit data without the need for
               physical cables.
    
    Examples -
    Wi-Fi
    Bluetooth 
    Cellular Network 
    Zigbee 

Communication media, or transmission media, are the physical pathways through which data is transmitted in a network. They
can be broadly categorized into two types:

1. Guided Media

Guided media provide a physical path for data transmission.

Twisted-Pair Cable:
Description: Two insulated copper wires twisted together to reduce interference.
Types:

![1973_1](https://github.com/user-attachments/assets/ac4cbe73-b755-4088-8703-c2ff59822094)
![Screenshot (695)](https://github.com/user-attachments/assets/905551cf-6e65-405e-b0df-5eb02436d669)


Shielded Twisted Pair (STP): Provides better shielding against interference.
Unshielded Twisted Pair (UTP): More common and less expensive.

Real-world Example: Ethernet cables used to connect computers to a router or switch.

Coaxial Cable:
Description: A single copper wire surrounded by insulation, a braided shield, and an outer jacket.
Types:
Baseband coaxial cable
Broadband coaxial cable

![Screenshot (696)](https://github.com/user-attachments/assets/afc2e594-0b80-48ca-934d-e6ab7ec4b71c)

Real-world Example: Older cable TV networks and some older Ethernet networks.

Fiber Optic Cable:
Description: Uses thin strands of glass or plastic to transmit data as pulses of light.
![Screenshot (697)](https://github.com/user-attachments/assets/cc717f44-0c26-45ad-93c2-de2b0d38beb1)

Types:
Single-mode fiber
Multi-mode fiber
Real-world Example: Long-distance telecommunications and high-speed internet connections.

2. Unguided Media

Unguided media transmit data through the air or space without a physical conductor.

Wireless Media:

Radio Waves: Used for Wi-Fi, Bluetooth, Zigbee, cellular networks, and radio broadcasts.

![radiowave](https://github.com/user-attachments/assets/ddd60451-3adb-4671-aca7-7157b301db9c)

Microwaves: Used for satellite communication and point-to-point links.

![Microwave-tranmission-media](https://github.com/user-attachments/assets/36300b80-6017-4fce-a934-8fea4dd7ee6f)

Infrared: Used for short-range communication, such as remote controls.

![infrared1-227x300](https://github.com/user-attachments/assets/a0dfc6b6-088c-41e4-a4a0-fb83e81a55d2)

Real-world Example: Wi-Fi networks in offices, homes, and public places.

![Screenshot (698)](https://github.com/user-attachments/assets/2b65785a-1e09-489f-9eac-ece72425c7b2)

Wi-Fi Protocols
- WEP (Wired Equivalent Privacy) early encryption standard, now outdated due to weak encryption.
- WPA (Wi-Fi Protected Access) Introduced to address WEP weaknesses with better encryption (TKIP temporal key integrity protocol ).
- WPA2 (Wi-Fi Protected Access 2) Uses AES encryption, significantly more secure than WEP and WPA.
- WPA3 (Wi-Fi Protected Access 3) The latest, offering enhanced encryption (AES-256) and security, ideal for modern networks.

Zigbee

Zigbee is a wireless communication protocol designed for low-power, low-data-rate applications.
It's particularly well-suited for home automation and IoT devices due to its low cost, long battery life, and reliable
mesh network capabilities.


Applications of Zigbee

- Home Automation: Controlling lights, thermostats, and other home appliances.   
- Smart Buildings: Monitoring and controlling building systems, such as HVAC and lighting.   
- Industrial Automation: Monitoring and controlling industrial processes.   
- Healthcare: Remote patient monitoring and medical device control.   
- Agriculture: Monitoring soil moisture, temperature, and other environmental factors.

Choosing the Right Media

The choice of communication media depends on several factors, including:

- Distance: Longer distances often require fiber optic cables or wireless technologies.
- Bandwidth: High-bandwidth applications need high-speed media like fiber optic cables.
- Security: Fiber optic cables are more secure than wireless or copper cables.
- Cost: Fiber optic cables are generally more expensive to install and maintain than copper cables.
- Environmental Factors: Wireless signals can be affected by obstacles and interference

# 1.9 Network Bandwidths
**Network bandwidth** is the maximum amount of data that can be transmitted over a network connection in a given amount of time,
usually measured in bits per second (bps), kilobits per second (Kbps), megabits per second (Mbps), or gigabits per second (Gbps).

It’s like the width of a highway: the wider the highway (or higher the bandwidth), the more cars (data packets) it can carry 
simultaneously, resulting in faster data transfer rates.

**Working Examples of Network Bandwidth**

**1. Home Internet Connection**

Example: Imagine a 100 Mbps home internet connection from a provider like Comcast or Verizon. This bandwidth rating means that
under ideal conditions, the connection can transfer up to 100 megabits of data per second.

Explanation: If only one device (like a laptop) is using the internet, it might use a large portion of that 100 Mbps bandwidth,
allowing for high-definition streaming, gaming, or large downloads. However, if multiple devices (smart TVs, phones, tablets, etc.)
are connected simultaneously, each device's speed will be slower as the 100 Mbps bandwidth is divided among them.

**2. Video Streaming on Platforms like Netflix or YouTube**

Example: Streaming services like Netflix recommend a minimum bandwidth of around 5 Mbps for HD video and up to 25 Mbps for 4K
UHD streaming.

Explanation: If you have a 10 Mbps connection, streaming HD content should work smoothly. However, if another device starts a
large download or someone else streams a video, the available bandwidth might fall below the 5 Mbps required for HD, resulting
in buffering or reduced video quality. Higher bandwidth connections allow multiple devices to stream high-quality video without
interruption.

**3. Corporate Office with High Bandwidth Needs**

Example: A company might have a 1 Gbps (1000 Mbps) connection to support hundreds of employees. In this case, employees require
internet for video conferencing, cloud computing, file sharing, and general browsing.

Explanation: The high bandwidth ensures that activities requiring significant data transfer, like video conferencing or accessing
large cloud-stored files, can be done without network slowdowns. However, if network activity spikes (e.g., everyone is streaming
a video or uploading files simultaneously), even 1 Gbps may feel limited, causing delays.

**4. Online Gaming**

Example: Online games require a stable internet connection with low latency and sufficient bandwidth. For example, games like
Fortnite or Call of Duty may require at least 3 Mbps for optimal performance.

Explanation: Though online gaming doesn’t use much bandwidth compared to streaming, it requires a steady connection. Low
bandwidth can cause lag, especially when other devices are streaming or downloading large files. Gamers often use high-bandwidth
connections to avoid interruptions.

**5. Cloud-Based Applications**

Example: Cloud-based applications like Google Workspace, Microsoft Teams, or Zoom require considerable bandwidth, especially
for video calls or file sharing.

Explanation: A bandwidth of around 10-20 Mbps per user is recommended for smooth video calls. If bandwidth is low, calls may
experience lag or freeze, while files may upload/download slowly. High bandwidth ensures that employees can interact without
disruptions, even during peak usage.

**6. IoT Devices and Smart Homes**

Example: Smart home setups with multiple devices like security cameras, smart lights, and thermostats use network bandwidth to
send and receive data.

Explanation: Security cameras, especially high-definition ones, can use significant bandwidth for video uploads. In a network
with limited bandwidth, having multiple IoT devices connected can slow down the network. Higher bandwidth prevents smart home
devices from disrupting one another or other connected devices.

Why Network Bandwidth Matters

Bandwidth affects:

- Data transfer speed: Higher bandwidth allows more data to be transferred quickly, which improves loading times and reduces
   buffering.
- Number of devices: Networks with higher bandwidth can support more devices and activities simultaneously.
- Quality of experience: Insufficient bandwidth can result in lower video quality, longer loading times, and reduced
   efficiency, especially for critical applications like video calls.

**Related Terminologies -**

1. Broadband

Definition: Broadband is a method of data transmission that uses a wide range of frequencies, enabling the simultaneous
transmission of multiple data signals.

Example: Cable internet, DSL, and fiber-optic connections are types of broadband. Broadband allows multiple channels within
the frequency band, so users can download, upload, stream, and browse simultaneously.

Application: Broadband is ideal for high-speed internet connections as it supports multiple data streams (e.g., video calls,
web browsing, gaming) at the same time.

2. Baseband

Definition: Baseband is a transmission method that uses the entire bandwidth of the communication channel for a single data
signal. It’s unidirectional and supports only one data stream at a time.

Example: Ethernet networks use baseband transmission, where only one device can transmit data at a time on the network medium.

Application: Baseband is typically used in local area networks (LANs) because it’s simpler and cheaper but effective for short-range
communication where only one device transmits at a time.

3. Latency

Definition: Latency refers to the delay between when data is sent and when it’s received. It’s usually measured in milliseconds (ms).

Example: In a video call, high latency can lead to noticeable lag or delay between when one person speaks and when the other hears it.

Application: Low latency is crucial for real-time applications like gaming, video conferencing, and live streaming, where even small
delays can disrupt the user experience.

4. Throughput

Definition: Throughput is the actual amount of data successfully transmitted over the network in a given time. While bandwidth is the
maximum data transfer capacity, throughput is the actual data transfer rate, usually less than bandwidth.

Example: If a network has 100 Mbps bandwidth but experiences interference, it might have a throughput of only 80 Mbps.

Application: Network performance measurements often consider throughput to assess how efficiently a network is using its available bandwidth.

5. Bandwidth

Definition: Bandwidth is the maximum data transfer rate of a network, measured in bits per second (bps). It defines the total amount of data
that can be transferred over a network in a set period.

Example: A 1 Gbps (gigabit per second) Ethernet connection has a maximum bandwidth of 1 billion bits per second.

Application: Higher bandwidth allows more data to flow, supporting activities like high-definition video streaming,
large file transfers, and multiple simultaneous connections.

6. Bit Rate

Definition: Bit rate is the number of bits transmitted per second in a network. It’s a measure of data transfer speed and is often used
interchangeably with bandwidth.

Example: A music streaming service with a 320 Kbps bit rate transmits 320 kilobits of data per second for high-quality sound.

Application: Bit rate is significant for digital media (audio and video) quality, where higher bit rates correspond to better quality
but require more bandwidth.

7. Packet Loss

Definition: Packet loss occurs when data packets traveling over a network fail to reach their destination. It’s often caused by network
congestion, hardware failures, or signal interference.

Example: During a video call, packet loss can cause frozen screens or distorted audio, as some of the data fails to transmit successfully.

Application: Low packet loss is essential for applications requiring consistent data flow, like VoIP (Voice over IP) and online gaming.
High packet loss can significantly degrade the quality of these applications.

8. Jitter

Definition: Jitter refers to the variation in packet arrival times, which can disrupt the smooth flow of data. It’s particularly problematic
for time-sensitive communications.

Example: In a video call, jitter can result in choppy audio or misaligned video and audio.

Application: Networks often measure and attempt to minimize jitter for video and voice applications, where data needs to arrive in a specific
order and timing.

9. Full Duplex and Half Duplex

Full Duplex: Communication in which data transmission occurs simultaneously in both directions.
Example: Modern Ethernet networks and phone lines support full-duplex communication, allowing seamless conversations without waiting turns.

Half Duplex: Communication in which data transmission occurs in both directions but not at the same time.
Example: Walkie-talkies are half-duplex devices where only one person can speak at a time, while the other listens.

Application: Full-duplex communication is generally preferred in networking as it increases efficiency, particularly in fast data transfer
environments like gigabit Ethernet networks.

10. Signal-to-Noise Ratio (SNR)

Definition: Signal-to-noise ratio is the measure of the signal strength relative to background noise on a network. Higher SNR means better
signal quality.
Example: In Wi-Fi networks, a low SNR can reduce speeds and increase the chance of dropped connections.
Application: High SNR is essential in wireless networks to ensure clear, reliable data transmission, particularly in environments with
interference from other wireless devices.

11. Data Rate and Baud Rate

Data Rate: Refers to the number of data bits (binary bits) transmitted per second in a network.
Baud Rate: The number of signal changes per second in a communication channel.
Example: In modems, a baud rate of 2400 can carry a data rate of up to 9600 bps by encoding multiple bits in each signal change.
Application: Baud rate is significant for analog communication channels, while data rate is relevant for measuring digital
communication speeds.

12. Latency vs. Bandwidth
Latency measures the delay in data transmission, while bandwidth measures the capacity of the network connection.
Example: A network with high bandwidth but high latency might allow large downloads but would struggle with real-time applications
like gaming, where quick response times are needed.

# 1.10 Ethernet Cable Color Coding
**RJ45 Wiring Standards (T568A and T568B)**

The two standard wiring configurations, T568A and T568B, define how the colored wires are arranged in an RJ45 connector for standard Ethernet cabling:

**T568A Wiring Standard**

- Pin 1: White/Green
- Pin 2: Green
- Pin 3: White/Orange
- Pin 4: Blue
- Pin 5: White/Blue
- Pin 6: Orange
- Pin 7: White/Brown
- Pin 8: Brown

**T568B Wiring Standard**

- Pin 1: White/Orange
- Pin 2: Orange
- Pin 3: White/Green
- Pin 4: Blue
- Pin 5: White/Blue
- Pin 6: Green
- Pin 7: White/Brown
- Pin 8: Brown

T568B is the most widely used standard, especially in the United States, while T568A is sometimes used in government and residential networks.


1. Straight-Through Cabling
**Application:** Used to connect different types of devices, like computers to switches or routers.

**Example:** In an office, straight-through cables connect workstations to the network switch, allowing communication over the LAN.

**Wiring:** T568B on both ends (or T568A for residential).

![Screenshot (699)](https://github.com/user-attachments/assets/414041cb-0542-4830-a2d5-b68a724e1a7f)

![Screenshot (700)](https://github.com/user-attachments/assets/60c766d8-8ba2-4f5a-b03f-7dbbc783d31f)

2. Cross-Over Cabling
**Application:** Connects similar devices directly, like two computers or two switches without an intermediary device.

**Example:** A crossover cable can be used to connect two laptops for direct file sharing without a network switch.

**Wiring:** T568A on one end, T568B on the other.

![Screenshot (701)](https://github.com/user-attachments/assets/14a8768d-05c6-4483-a53e-8a967a3183a3)

![Screenshot (702)](https://github.com/user-attachments/assets/854aa7ac-bc01-47ca-a87e-774609f4f2ec)


3. Console (Roll over) Cabling
**Application:** Primarily used to connect a computer to the console port of a networking device like a router or switch for configuration.

**Example:** Network administrators use a rollover cable to connect a laptop to a Cisco router’s console port to configure it.

**Wiring:** Pin 1 to Pin 8, Pin 2 to Pin 7, Pin 3 to Pin 6, etc. (the cable is “rolled over” so the pins on one side are reversed on the other).

The rollover cable is wired in reverse:

- Pin 1 to Pin 8
- Pin 2 to Pin 7
- Pin 3 to Pin 6
- Pin 4 to Pin 5
- Pin 5 to Pin 4
- Pin 6 to Pin 3
- Pin 7 to Pin 2
- Pin 8 to Pin 1
![Rollover-Cable](https://github.com/user-attachments/assets/4a6c5722-0b01-47ee-95ec-8d8d7b15af49)

5. Power over Ethernet (PoE) Applications
**Application:** Combines data and power over a single Ethernet cable, ideal for powering devices like IP cameras, phones, and wireless access points.

**Example:** In an office, PoE allows installation of security cameras and access points without needing separate power sources.

**Wiring:** Either T568A or T568B, based on the environment.

