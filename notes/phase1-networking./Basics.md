# Networking Basics

## OSI Model

### What is it?

The **OSI (Open Systems Interconnection)** Model is a conceptual framework that explains how devices communicate over a network. It divides communication into **7 layers**, where each layer performs a specific function.

---

### Why is it Important?

- Provides a standard way to understand network communication.
- Makes troubleshooting easier.
- Helps identify where network or security issues occur.
- Forms the foundation of networking and cybersecurity.

---

### The 7 Layers

| Layer | Name | Main Function |
|-------|--------------|----------------------------------|
| 7 | Application | Provides network services to users and applications. |
| 6 | Presentation | Formats, encrypts, and compresses data. |
| 5 | Session | Establishes, manages, and terminates communication sessions. |
| 4 | Transport | Ensures reliable or fast data delivery. |
| 3 | Network | Routes packets using IP addresses. |
| 2 | Data Link | Handles communication within a local network using MAC addresses. |
| 1 | Physical | Transmits bits through cables or wireless signals. |

---

### Common Protocols & Technologies

| Layer | Protocols / Technologies |
|-------|--------------------------|
| Application | HTTP, HTTPS, DNS, DHCP, FTP, SSH, SMTP |
| Presentation | SSL/TLS |
| Session | NetBIOS, RPC |
| Transport | TCP, UDP |
| Network | IP, ICMP |
| Data Link | Ethernet, ARP, MAC Address |
| Physical | Ethernet Cable, Fiber Optic, Wi-Fi |

---

I think its like a company where each department has a different job , and together they ensure that the package reaches to the correct destination . If anything goes wrong , the model helps identify exactly where the problem occured .

---
## TCP/IP Model

### What is it?

The TCP/IP model is the networking model used by the internet. It defines how devices communicate and exchange data across networks.

### The 4 Layers

| Layer | Purpose |
|---------|---------|
| Application | Network services used by applications |
| Transport | End-to-end communication |
| Internet | Routing packets between networks |
| Network Access | Physical transmission and local network communication |

### OSI vs TCP/IP

| OSI | TCP/IP |
|------|---------|
| 7 Layers | 4 Layers |
| Learning model | Real-world model |
| More detailed | Simpler |
| Used for understanding networks | Used by the internet |

### Common Protocols

| Layer | Examples |
|---------|---------|
| Application | HTTP, HTTPS, DNS, FTP, SMTP, SSH |
| Transport | TCP, UDP |
| Internet | IPv4, IPv6, ICMP |
| Network Access | Ethernet, Wi-Fi, ARP |

### Why its useful ?

Most logs, packet captures, and security alerts are based on TCP/IP communication. Understanding this model helps analyse network traffic.

### My Understanding

OSI helps in understand networking concepts, while TCP/IP is what devices actually use to communicate.

---

## TCP vs UDP

### What are they?

TCP and UDP are Transport Layer protocols responsible for moving data between devices.

### TCP (Transmission Control Protocol)

#### Features

- Connection-oriented
- Reliable delivery
- Uses acknowledgements
- Detects lost packets
- Packets arrive in order

#### Common Uses

- HTTP
- HTTPS
- SSH
- FTP
- Email
---

### UDP (User Datagram Protocol)

#### Features

- Connectionless
- No acknowledgement
- No guarantee of delivery
- Faster than TCP

#### Common Uses

- DNS
- VoIP
- Online gaming
- Video streaming

---

### TCP vs UDP Comparison

| Feature | TCP | UDP |
|----------|----------|----------|
| Connection | Yes | No |
| Reliable | Yes | No |
| Speed | Slower | Faster |
| Error Checking | Extensive | Minimal |
| Packet Ordering | Yes | No |

### Example

TCP is like sending a registered courier where delivery is confirmed.

UDP is like making a public announcement through a loudspeaker. It is fast, but there is no guarantee everyone hears it.

### Why its imp bcz.

Understanding whether traffic uses TCP or UDP helps during packet analysis and incident investigations.

Examples:
- Multiple failed TCP connections may indicate scanning activity.
- Large volumes of UDP traffic may indicate DNS abuse or amplification attacks.

- Both operate at the Transport Layer.
- Many security investigations involve analysing TCP and UDP traffic.

### My Understanding

If data must arrive correctly, TCP is used. If speed is more important than reliability, UDP is usually preferred.
