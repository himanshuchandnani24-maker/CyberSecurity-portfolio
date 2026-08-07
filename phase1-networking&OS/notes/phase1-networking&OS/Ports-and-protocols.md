# Ports and Protocols

## DNS

### What is DNS?
DNS (Domain Name System) translates domain names like `google.com` into IP addresses so devices can find websites.

### Key Points:
- Internet's phonebook
- Uses Port 53 (TCP/UDP)
- Converts names to IP addresses

### Why it matters
Almost every website visit starts with a DNS lookup. Suspicious DNS requests are often investigated during security incidents.

---

## HTTP vs HTTPS

### HTTP
- Sends data in plain text
- Uses Port 80
- Not secure

### HTTPS
- Uses TLS/SSL encryption
- Uses Port 443
- Protects sensitive information

### Quick Comparison

| HTTP | HTTPS |
|------|-------|
| No encryption | Encrypted |
| Port 80 | Port 443 |
| Less secure | More secure |

### Why it matters
Always prefer HTTPS because it protects data from being intercepted.

---

## SSH, FTP & RDP

### SSH (22)
- Secure remote access
- Encrypted
- Used by administrators

### FTP (21)
- Transfers files
- Not encrypted
- Mostly replaced by SFTP/FTPS

### RDP (3389)
- Remote Windows desktop access
- Common target for brute-force attacks

### Why it matters
Attackers frequently target SSH and RDP services. Exposed FTP servers can also become a security risk.

---

## Firewalls

### What is a Firewall?
A firewall monitors and filters network traffic based on security rules.

### What it can filter
- IP addresses
- Ports
- Protocols
- Incoming traffic
- Outgoing traffic

### Example
Allow HTTPS (443) but block FTP (21) if it isn't needed.

### Why it matters
Firewalls help prevent unauthorized access and reduce the attack surface.
