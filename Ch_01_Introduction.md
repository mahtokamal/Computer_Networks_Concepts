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
    - If a user had to print a document, he would need to copy the file to a removable media (Floppy Disks), move to the PC that was
      connected to the Printer, open the file from the Floppy and print it.
    - This is where network helped by connecting the devices (Computers, Printers etc.) to each other so that these resources could
      be shared with each other.


    Any device which can share or receive the data is called a Node. 
    Through which the information or data propagate is known as channels, It can be guided or unguided.
    
    Goal of Networking
    - Shared hardware such as printers and input devices
    - Shared data and information through the use of shared storage devices
    - Communications such as email, instant messaging, chat rooms, etc.
    - Shared software, which is achieved by running applications on remote computers (Google GSuites, Microsoft office 365, Dropbox, GMail)

    wired Network - Cables consist of Coaxial, UTP, STP, Fibre Optics . Centralized devices will be Switch or Hub. Nowadays, Switch is preferred.
   
    Wireless Network - Radio waves or frequency. It uses Wireless Access Point device (equivalent to Switch in wireless networking).

    Hybrid Network - uses both wired and wireless devices. The Wireless Access Point Connects to the Switch using a Cable.
            The access point acts as a connection bridge between a wired and a wireless network.

    NIC - network interface card. Wi-Fi connections use wireless NICs (WLAN). Ethernet is the most popular wired LAN technology.
    RG-58 - Coaxial Cable connectore. BNC connector for RG58 cable. (Bayonet Neil-Concelman, or sometimes British Naval Connector) connector 
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

    1. Hub -  It works on OSI Layer 1.A hub is a basically multi-port repeater. Hubs cannot filter data, so data packets are
              sent to all connected devices. In other words, the collision domain of all hosts connected through Hub remains
              one Hub. It is an unintelligent device that forwards the signal to all other ports and received by all connected
              devices, as a result all devices gets the unnecessary network traffic and causes network bandwidth problems.  
    
    2. Repeater - Operates at OSI Layer 1 i.e. Physical Layer. It just amplifies (or regenerate) the signal within a same network
                  before the signals become too weak or corrupted to to extend the length to which the signal can be transmitted over
                  the same network. When the signal becomes weak, they copy it bit by bit and regenerate it at its star topology
                  connectors connecting following the original strength.
    
    3. Bridge - A bridge operates at the OSI Layer 2 i.e. Data Link Layer. A bridge is a repeater, with add on the functionality
                of filtering content by reading the MAC addresses of the source and destination. It is also used for interconnecting
                two LANs working on the same protocol.
    
    4. Switch (Layer 2 or Layer 3) - It works on OSI Layer 2 and uses MAC address(Media Access Control or Physical Address) of device
                                     to sends or forward the data to the another device to the destination device
                                     (destination device's MAC address) within a same network typically (LAN). It is an intelligent
                                     device as compared to Hubs. A switch is a multiport bridge with a buffer and a design that can boost
                                     its efficiency(a large number of ports imply less traffic) and performance. The switch can perform
                                     error checking before forwarding data, which makes it very efficient as it does not forward packets
                                     that have errors and forward good packets selectively to the correct port only.  In other words, the
                                     switch divides the collision domain of hosts, but the broadcast domain remains the same.

       Managed - Managed Switch have lots of option depending upon switch.
                 It has better security. We can segment our network into different VLAN, with some ports on one VLAN and other ports
                 on different VLAN. For example - put IoT devices into one VLAN and PCs into other VLANs segment each other so that
                 they can't communicate with each other.
                
       Unmangaed Switch - These are lot cheaper than managed switches. It comes with very limited features that are only provided by
                          Venodrs. In this, we can't change the configuration of the device. These are plug and play, gives ability to extend the network.
                          For example - if you plug ethernet cable to unmanaged switch port then you can connect more devices to the network.
       
       Layer 3 Switch - This switch can be used in routing and therefore, operates at OSI layer 3. It supports VLAN(Virtual Local Area
                        Network), VLAN is a Subnet and it routes the traffic from one subnet to another without a need of router locally.
    
    5. Modem - Modem stands for Modualtion and demodulation (analog to digital and digital to analog). A modem brings internet service
               into the home from internet service providers (ISPs). Some ISPs offer a combination of modem-router unit, known as a gateway.

               Most ISPs will either rent you a modem or sell you one outright. Many modems nowadays are "all-in-one" devices that also
               include a router, although you can still purchase a modem and router separately.

               There are three common types of modem connections:

               Dial-up — A modem that uses a phone line to connect to an ISP. This is the oldest type of modem connection and has largely
               been replaced by broadband connections.
               
               DSL — A digital subscriber line modem uses a phone line to connect to an ISP but with much higher speeds than dial-up.
               
               Cable — A modem that uses a cable TV line to connect to an ISP. This is the most common type of modem connection.
    
    6. Router - Works on OSI Layer 3 and routes the data from one network to other using IP address (Source and Destination).
                TP-Link router, has LAN ports(basically switch port). routes the traffic from LAN to WAN. 
                CISCO router, have switch ports and can act as a switch within LAN.
    
    7. Gateway -  A gateway, as the name suggests, is a passage to connect two networks that may work upon different networking models.
                  They work as messenger agents that take data from one system, interpret it, and transfer it to another system. Gateways
                  are also called protocol converters and can operate at any network layer. Gateways are generally more complex than switches
                  or routers.
    
    8. Brouter -  It is also known as the bridging router is a device that combines features of both bridge and router. It can work either
                  at the data link layer or a network layer. Working as a router, it is capable of routing packets across networks and working
                  as the bridge, it is capable of filtering local area network traffic.

    9. NIC - NIC or network interface card is a network adapter that is used to connect the computer to the network. It is installed in the
             computer to establish a LAN.  It has a unique id that is written on the chip, and it has a connector to connect the cable to it.
             The cable acts as an interface between the computer and the router or modem. NIC card is a layer 2 device which means that it
             works on both the physical and data link layers of the network model.




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

## 1.5 TCP/IP vs OSI Layer

![Screenshot (630)](https://github.com/user-attachments/assets/2eaa585a-3cde-4704-b493-90fd706200a6)

## 1.5 The Internet & DNS
    The Internet - ISP 
    
    
    Basics Services / Protocols on the Internet - Web Services(Web Server or WWW), Email Service(SMTP), Name Services(DNS)
    
    DNS
    
    DNS Communication Process
