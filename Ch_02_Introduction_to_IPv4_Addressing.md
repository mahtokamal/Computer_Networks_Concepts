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
    - You start from left to right. Put a 1 for the bit value as long as you don’t exceed the Decimal number.
      For the 199, I put a “1” in the 128 bit but a “0” for the 83.
    - Subtract the bit value from the Decimal number and move to the next bit.

    - Let’s convert 1011 0110. 0101 1100.1100 0111.0001 1011 into Decimal.
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

## 2.3 Private IPv4 Addressing
