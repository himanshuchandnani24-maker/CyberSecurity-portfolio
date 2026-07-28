# Networking Basics

## 1. OSI Model

### What is it?
The OSI (Open Systems Interconnection) model is a conceptual framework that explains how data moves between devices over a network. It divides communication into seven layers, each responsible for a specific task.

### 7 Layers

| Layer | Purpose | Examples |
|-------|---------|----------|
| 7. Application | User-facing network services | HTTP, HTTPS, DNS |
| 6. Presentation | Data formatting, encryption | TLS/SSL |
| 5. Session | Starts and manages sessions | NetBIOS |
| 4. Transport | Reliable or fast delivery | TCP, UDP |
| 3. Network | Routing packets | IP, ICMP |
| 2. Data Link | Local communication | Ethernet, MAC |
| 1. Physical | Transmits bits | Cables, Wi-Fi |

### Key Points
- Data moves from Layer 7 → Layer 1 when sending.
- The receiver processes it from Layer 1 → Layer 7.
- Each layer performs one specific task.

### Why It Matters
Understanding the OSI model helps troubleshoot network problems and identify where an attack or failure is occurring.

____
I think of the OSI model as a delivery company where each department has one job before the package reaches its destination.

---

## 2. TCP/IP Model + TCP vs UDP

### TCP/IP Model

The TCP/IP model is the networking model used on the internet. Unlike OSI, it has only four layers.

1. Application
2. Transport
3. Internet
4. Network Access

### TCP vs UDP

| TCP | UDP |
|-----|-----|
| Connection-oriented | Connectionless |
| Reliable | Faster |
| Uses acknowledgements | No delivery confirmation |
| Web browsing, Email | Streaming, Gaming, VoIP |

### Key Points
- TCP performs a three-way handshake before communication.
- UDP sends data without checking delivery.
- Choose TCP for reliability and UDP for speed.

### Why It Matters
SOC analysts often identify suspicious traffic based on whether TCP or UDP is being used.

___
TCP values reliability, while UDP values speed.

---

## 3. MAC Address vs IP Address

### MAC Address
- Physical hardware address
- Unique to the network interface
- Used inside a local network
- Usually doesn't change

### IP Address
- Logical address
- Used to communicate across different networks
- Can change depending on the network

### Easy Analogy
- MAC = Your fingerprint
- IP = Your current home address

### Why It Matters
MAC identifies the device, while IP identifies where the device is on the network.

---

## 4. NAT (Network Address Translation)

### What is it?
NAT allows multiple devices in a private network to share one public IP address when accessing the internet.

### How it Works
Private IP → Router (NAT) → Public IP → Internet

### Why It Exists
- Conserves public IPv4 addresses.
- Hides internal IP addresses from the internet.
- Makes home and office networks possible.

___
The router acts like a receptionist, translating requests between private devices and the internet.

---

## 5. DHCP

### What is it?
DHCP automatically assigns network settings to devices when they join a network.

### What It Assigns
- IP Address
- Subnet Mask
- Default Gateway
- DNS Server

### DHCP Process
1. Discover
2. Offer
3. Request
4. Acknowledge (DORA)

### Why It Matters
Without DHCP, every device would need manual network configuration.

___
DHCP works like a hotel receptionist assigning rooms to new guests automatically.
