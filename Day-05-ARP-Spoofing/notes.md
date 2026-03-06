# Day 5 – ARP Spoofing (Man-in-the-Middle Attack)

## Why ARP is Vulnerable
ARP does not have authentication.
Devices trust any ARP reply on the network.

## What is ARP Spoofing
ARP spoofing is when an attacker sends fake ARP messages to associate their MAC address with another device's IP address.

## Example
Victim IP: 192.168.1.10
Router IP: 192.168.1.1

Attacker sends a fake ARP reply saying:
192.168.1.1 → Attacker MAC

Now the victim sends traffic to the attacker instead of the router.

## Man-in-the-Middle Attack
The attacker sits between the victim and the router.

Traffic flow:
Victim → Attacker → Router

The attacker can monitor, modify, or intercept the data.

## Key Point
ARP spoofing works because ARP does not verify the authenticity of ARP replies.
