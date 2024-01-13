Opened the **** interface in wireshark and protocols traced were following:
- SSDP: Simple Service Discovery Protocol
- ICMP: Internet Control Message Protocol
- ARP: Address resolution Protocol
- DNS: Domain Name system
- TCP: Transmission Control protocol
- TLS: Transport Layer Security

I Sent request to 3 websites using HTTP and capture the packets using Wireshark as mentioned below

Website | IP & Mac Source Address | IP & Mac Destination Address | Http response code| Round Trip Time for http 200|Http response code after reloading | Round trip time after reloading|Transport layer protocol(tcp/udp)|Source(client) port|Desination(server) port 
--------|--------------|----------------|-------------------|----------|-----|------|------|-----|---------
http://www.example.com|172.22.45.7- 08:00:27:cb:7e:f5|93.184.216.34- 00:15:5d:59:c7:03 |200|0.543665463 sec|304|0.227996837 |TCP|41010|80 |
