# 1. Introduction to Networking

## 1.1 Introduction to Networks
    What is Network?
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
    LAN -  Local Area Network
    MAN - Metropolitan Area Network
    WAN (Private) - Wide Area Network
    WAN (Public) Internet -
    

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
    Star
    Bus
    Ring
    Mesh
    Hybrid

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
    
             Function -
             Devices -
             Secure protocol -
             unsecure protocol -
             Attack scenario -
             prevention mechanism -
             Defense against attack -
    
    Layer 6: Presentation layer
             Function -
             Devices -
             Secure protocol -
             unsecure protocol -
             Attack scenario -
             prevention mechanism -
             Defense against attack -
    
    Layer 5: Session layer ()
             Function -
             Devices -
             Secure protocol -
             unsecure protocol -
             Attack scenario -
             prevention mechanism -
             Defense against attack -
    
    Layer 4: Transport layer (Data = Segments)
    
             Function -
             Devices -
             Secure protocol -
             unsecure protocol -
             Attack scenario -
             prevention mechanism -
             Defense against attack -
    
    Layer 3: Network layer (Data = Packets)
             Function -
             Devices -
             Secure protocol -
             unsecure protocol -
             Attack scenario -
             prevention mechanism -
             Defense against attack -
    
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

## 1.5 The Internet & DNS
    The Internet - ISP 
    
    
    Basics Services / Protocols on the Internet - Web Services(Web Server or WWW), Email Service(SMTP), 
    Name Services(DNS)
    
    DNS - Domain Name System
    
    DNS Communication Process

## 1.6 Network Ports
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

## Communication Medias
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


    

