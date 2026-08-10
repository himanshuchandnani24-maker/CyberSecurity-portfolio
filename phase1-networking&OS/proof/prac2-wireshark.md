# Practical 2 - Wireshark

- Wireshark was used to capture and analyze network packets from the active network interface.

![DNS filter](prac2-wireshark(a).png)
- The `dns` filter was used to view and analyze DNS packets.

![HTTP/TLS filter](prac2-wireshark(b).png)
- The `tls`/`http` filter was used to identify web traffic generated while visiting a website.

![TCP SYN filter](prac2-wireshark(c).png)
- The `tcp.flags.syn==1` filter was used to identify TCP SYN packets used to establish a TCP connection.
