Opened the **** interface in wireshark and protocols traced were following:
- SSDP: Simple Service Discovery Protocol
- ICMP: Internet Control Message Protocol
- ARP: Address resolution Protocol
- DNS: Domain Name system
- TCP: Transmission Control protocol
- TLS: Transport Layer Security

I Sent request to 3 websites using HTTP and capture the packets using Wireshark as mentioned below

Website | Address Type | Source Address | Destination Address | Http response code| Round Trip Time for http 200|Http response code after reloading | Round trip time after reloading|Transport layer protocol(tcp/udp)|Source(client) port|Desination(server) port 
--------|--------------|----------------|-------------------|-----|-------|-----|------|------|-----|---------
