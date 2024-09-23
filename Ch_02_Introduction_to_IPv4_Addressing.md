# 2.0 Introduction to IPv4 Addressing

## 2.1 IPv4 Addressing
    IP Addressing Overview
    - Most of the devices on the Internet communicate to each other using a Protocol called the Internet Protocol (IP). Most
      of the Internet is running Version 4 of the IP Protocol.
    - Every device on the Internet has to be identified uniquely on the Internet. This is done by assigning each device an Address. 
    - This Address is called the IPv4 address or an IP Address.
    - An IP address is a 32-bit number written in dotted decimal notation. [199.87.20.5]. 
    - Each digit is a 8-bit value separated by a “ . ”. This 8-bit block is known as an Octet.
    - The IP address has 4 Octets.
    - The total size of an IP Address is 32 Bits. 
    
    Binary & Decimal Numbering Systems
    - Although the IP address is written in decimal, the devices process it in the Binary System.
    - We have 8 bits in each Octet. 
    - It is important to understand the conversion between Binary and Decimal within the Octet.
    - The following table helps in the conversion. 
    - In this table, the value represents the bit value of the corresponding bit in the IP Address.

| 128 | 64 | 32 | 16 | 8| 4 | 2 | 1 |
|--   |--  |--  |--  |--| --| --| --|
|     |    |    |    |  |   |   |   |
|     |    |    |    |  |   |   |   |

    Conversion Examples
    - Let’s convert the address 199.83.20.5 to Binary using the Table.
| Decimal #| 128 | 64 | 32 | 16 | 8| 4 | 2 | 1 |
|--|--   |--  |--  |--  |--| --| --| --|
|199| 1    |  1  |  0  | 0   | 0 | 1  |  1 | 1  |
|83|   0  |  1  |   0 |   1 | 0 | 0  | 1  | 1  |
|20|    0 |   0 |   0 |   1 | 0 |  1 |   0| 0  |
|5|   0  | 0   | 0   | 0   | 0 |  1 | 0  | 1  |
    - You start from left to right. Put a 1 for the bit value as long as you don’t exceed the Decimal number.
      For the 199, I put a “1” in the 128 bit but a “0” for the 83.
    - Subtract the bit value from the Decimal number and move to the next bit.

    - Let’s convert 1011 0110. 0101 1100.1100 0111.0001 1011 into Decimal.
| Decimal #| 128 | 64 | 32 | 16 | 8| 4 | 2 | 1 |
|--|--   |--  |--  |--  |--| --| --| --|
|182| 1    |  0 |  1  | 1  | 0 | 1  |  1 | 0 |
|92|   0  |  1  |   0 |   1 | 1 | 1  | 0  | 0  |
|199|    1 |   1 |   0 |   0 | 0 |  1 |   1| 1  |
|27|   0  | 0   | 0   | 1   | 1 |  0 | 1  | 1  |
    - Write the binary numbers into the table. 
    - Add the bit values that have a “1” in the column. For 182, add the 128 + 32 + 16 + 4 + 2 = 182.

    
    IPv4 Address & Subnet Mask
    - he IP Address has 2 parts, network and Host.
    - This is similar to a street address. 
    - If we look at the address 150 Tasman Drive, it has the house number and the street name.
    - All the buildings on Tasman Drive will have Tasman Drive in their address. Each building will be identified with a unique
      building number.
    - Similarly, each device on a network will have a common Network address and a unique device address. The common address is
      known as the Network address whereas the device address is known as a Host address.
    - The Network address versus the Host address is identified by an accompanying address known as the Subnet mask.

    - Example: 199.87.50.5 is an address assigned to a device and the associated mask is 255.255.255.0. The 255 decimal number
      identifies the Network portion and 0 represents the host portion. All  the devices on this network will have 199.87.50 in
      the first 3 octets with a unique address in the 4th Octet.
    - The subnet mask identifies the Network portion of the Address by setting the bit to 1 and the host portion by setting the
      corresponding bit to 0.
    - The 255 is representing the all the bits in the octet being 1’s.
    - The network bits have to be contiguous from left to right. 
    - Another way of representing the network portion is by identifying the number of network bits.
    - The 199.87.50.5 address with a subnet mask of 255.255.255.0 can also be written as 199.87.50.5/24.
    - The /24 specifies that the first 24 bits [first 3 octets] are the network bits.

    IPv4 Address Types
    Unicast
    - The most common type of IP address is the Unicast Address.
    - It normally refers to a single receiver.
    - A unicast address is associated with a single device or host.
    
    Broadcast
    - This address is used to send data to all possible destinations ("all-hosts broadcast"), which permits the sender to send
      the data only once, and all receivers receive a copy of it. 
    - The address 255.255.255.255 is used for sending data as a broadcast. 
    - In addition, a directed (limited) broadcast can be made by combining the network prefix with a host suffix composed
      entirely of binary 1s. For example, the destination address used for a directed broadcast to devices on the 192.0.2.0/24
      network is 192.0.2.255. 
    
    Multicast
    - A multicast address is associated with a group of interested receivers.
    - In IP, addresses 224.0.0.0 through 239.255.255.255 are designated as multicast addresses. 
    - The sender sends a single packet from its unicast address to the multicast group address and the intermediary routers
      take care of making copies and sending them to all receivers that are part of the group.

## 2.2 IPv4 Address Classes
     IPv4 Address Classes
     - IP addresses are split up into 4 main categories called Classes.
     - These Classes are identified as A, B, C & D.
     - The first 3 Classes [A, B & C] are used for Unicast communications [One-to-One] whereas the 4th class is used for
       Multicast communications [One-To-Many]. 
     - Multicast communications will be discussed later in the course.

     Class A
     - A Class A address has the following characteristics:
         The first bit of the Address is set to “0”.
         The first 8 bits represent the network bits, the next 24 bits are host bits. This is the default split between
         Network and Host bits.
     - There are less number of Class A networks in the world. Each one of the networks though has a lot of host on it. 
     - As the first bit is fixed as “0” in the first Octet, the range of class A address is from 0000 0001 – 0111 1111.
       [ 1 – 127].
     - If an IP Address has a number between 1 – 127 in the first Octet, it is a Class A address. 
     - You have a total of 127 Class A networks with a total of 16,777,214 hosts on each network.
     - As there are a lot of hosts on each network, the network administrator has the ability to borrow host bits and
       give them to the network bits. This is called Subnetting and will be discussed in detail.

    Class B
    - A Class B address has the following characteristics:
        The first 2 bits of the Address is set to “10”.
        The first 16 bits represent the network bits, the next 16 bits are host bits. This is the default split
        between Network and Host bits.
    - There are more Class B networks in the world. Each one of the networks though has a lesser number of hosts on
      each network.
    - As the first 2 bit are  fixed as “10” in the first Octet, the range of class B address is from
      1000 0000 – 1011 1111. [ 128 – 191].
    - If an IP Address has a number between 128 – 191 in the first Octet, it is a Class B address. 
    - You have a total of 16,384 Class B networks with a total of 65,534 hosts on each network.
    - The network administrator has the ability to borrow host bits and give them to the network bits. 

    Class C
    - A Class C address has the following characteristics:
        The first 3 bits of the Address is set to “110”.
        The first 24 bits represent the network bits, the next 8 bits are host bits. This is the
        default split between Network and Host bits.
    - There are more Class C networks in the world. Each one of the networks though has a lesser
      number of hosts on each network.
    - As the first 3 bit are  fixed as “110” in the first Octet, the range of class C address is
      from 1100 0000 – 1101 1111. [ 192 – 223].
    - If an IP Address has a number between 192 – 223 in the first Octet, it is a Class C address. 
    - You have a total of 2,097,152 Class C networks with a total of 254 hosts on each network.
    - The network administrator has the ability to borrow host bits and give them to the network bits.

    Class D
    - Class D addresses are used for multicasting applications. 
    - The first 4 bit are  fixed as “1110” in the first Octet.
    - The range of class D address is from 1110 0000 – 1110 1111. [ 224 – 239].
    - Class D addresses are 32-bit network addresses, meaning that all the values within the range of
      224.0.0.0 – 239.255.255.255 are used to uniquely identify multicast groups. 
    - There are no host addresses within the Class D address space, since all the hosts within a group
      share the group’s IP address for receiving purposes.

    IP Address - Summary
| Class| 1st Octet Classifier | Class Rule | Address Structure | Subnet Mask | Networks | Maximum Hosts|
|--    |--                    |--          |--                 |--           |--        | --           |
|A| 1 - 127 |0XXXXXXX |N.H.H.H| 255.0.0.0  | 126 | 16,777,214 [2^24 - 2] |
|B| 128 - 191 |10XXXXXX |N.N.H.H| 255.255.0.0  | 16,384 | 65,534 [2^16 -2] |
|C| 192 - 223 |110XXXXX |N.N.N.H| 255.0.0.0  | 2,097,152 | 254 [2^8 – 2] |
|D| 224 - 239 |1110XXXX |Multicast Address|
|E| 240 - 255 |1111XXXX | Reserved for Experimental and Research|



## 2.3 Private IPv4 Addressing
    IPv4 Address Assignment
    - IP Address Blocks are assigned to the ISP’s by Internet Assigned Numbers Authority (IANA).
    - The ISP in turn will assign IP Addresses to the clients which could be individual users or
      enterprises communicate to each other on the Internet. These addresses are known as Public Addresses.  
    - The Internet has grown beyond anyone's expectations. 
    - As a result of the explosion of the Internet, the IP Addresses are getting depleted. 
    - To counter this concern, IANA, reserved a certain set of addresses that could be used internally
      within the private networks. 
    - These addresses can be used for communications within a Private network. They are defined in a
      standards document called the RFC. The RFC number for Private addresses is RFC 1918.
    - These addresses cannot be used on the Internet. They are assigned within the Private network and
      translated to a Public address when the device wants to communicate to the Internet.

    Private IP Address & NAT
    - The ISP assigns Dynamic IP addresses to clients from a Pool of addresses. When the client is not
      using the address, the address is returned back to the pool. It can be re-used for another client
      that might require it at that moment.
    - This allows you to use Public addresses more efficiently.
    - If an individual has more devices in his premises like on a home network or office, the Private
      addresses can be used internally. They are used when the devices want to communicate to each other
      on the internal network.
    - When an internal device wants to communicate to a device on the Internet, the Private address
      is translated to the IP Address assigned to the device by the ISP.
    - This process is called NAT. Multiple internal devices can share the same Public IP address on the
      Internet. This allows you to conserve IP Addresses by assigning a single address for a multiple set
      of Internal addresses.
    - We will discuss NAT in detail in a later section.

    Class A Private IP Range
    - A single Class A address is reserved by IANA for use on the internal networks. 
    - The Class A network that is reserved for Internal communications only is the 10.0.0.0/8 address.
    - This addresses from this network cannot be used when communicating to devices on the Internet.
    - If a device using this address range wants to communicate to devices on the Internet, it will need
      to be translated using NAT.

    Class B Private IP Range
    - The following Class B networks are reserved by IANA for use on the internal networks:
         172.16.0.0/16 – 172.31.0.0/24 [16 Networks]
    - This address cannot be used when communicating to devices on the Internet.
    - If a device using this address wants to communicate to devices on the Internet, it will need to be
         translated using NAT.

    Class C Private IP Range
    - The following Class C networks are reserved by IANA for use on the internal networks:
        192.168.0.0/24 – 192.168.255.0/24 [256 Networks]
    - These network addresses cannot be used when communicating to devices on the Internet.
    - If a device using this address range wants to communicate to devices on the Internet, it will need
      to be translated using NAT.

    Private IP Address & NAT

    
