# Subnetting

## Subnet Masks + CIDR

### What is a Subnet Mask?

A subnet mask divides an IP address into two parts:
- **Network ID** – identifies the network.
- **Host ID** – identifies a device within that network.

It helps devices determine whether the destination is on the same network or a different one.

### What is CIDR?

CIDR (Classless Inter-Domain Routing) is a shorter way of writing a subnet mask.

Example:
- `/24` = `255.255.255.0`

The number after the slash tells us how many bits are used for the network portion of the IP address.

### Common CIDR Values

| CIDR | Subnet Mask | Total Addresses | Usable Hosts |
|------|-------------|-----------------|--------------|
| /8 | 255.0.0.0 | 16,777,216 | 16,777,214 |
| /16 | 255.255.0.0 | 65,536 | 65,534 |
| /24 | 255.255.255.0 | 256 | 254 |
| /30 | 255.255.255.252 | 4 | 2 |

### Example

Network: `192.168.1.0/24`

- Network Address: `192.168.1.0`
- First Usable IP: `192.168.1.1`
- Last Usable IP: `192.168.1.254`
- Broadcast Address: `192.168.1.255`

### Key Points

- A subnet mask separates the network and host portions of an IP address.
- CIDR is simply a shorter way to write a subnet mask.
- `/24` is one of the most commonly used subnet sizes in home and office networks.

### Why It Matters

Subnetting improves network organization, reduces unnecessary traffic, and makes IP address management more efficient.
____

Subnetting is like dividing a large apartment building into smaller blocks, making it easier to locate and manage each apartment.
