# Day 4 – MAC Address & ARP

## MAC Address
- MAC stands for Media Access Control Address.
- It is a unique hardware address of a network device.
- Works at OSI Layer 2 (Data Link Layer).
- Used for communication inside a local network.

Example:
00:1A:2B:3C:4D:5E

## MAC vs IP Address

MAC Address
- Works at Layer 2
- Identifies device inside LAN
- Assigned by manufacturer

IP Address
- Works at Layer 3
- Identifies device on network
- Assigned by network/ISP

## ARP (Address Resolution Protocol)

- ARP converts IP address to MAC address.
- Used when a device knows the IP but not the MAC address.

Example:
If a device wants to send data to 192.168.1.1  
It asks: "Who has this IP?"

The device replies with its MAC address.

## Key Point

ARP connects Layer 3 (IP) with Layer 2 (MAC).
## ARP Process

When a device wants to communicate with another device in a local network:

1. The sender knows the destination IP address.
2. It sends an ARP Request to the network:
   "Who has this IP address?"
3. The device with that IP responds with an ARP Reply containing its MAC address.
4. The sender stores this MAC address in the ARP table.
5. Communication starts using the MAC address.
