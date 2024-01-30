### Solution 1.

### Solution 2.
This is the ping request made to www.inria.fr and respective resopnse
  - a. ICMP packets do not have source port and destination port. Because ICMP is not a transport or above layer protocol.
    
    ICMP (Internet Control Message Protocol) operates at the network layer of the OSI model and is primarily used for diagnostic and error reporting purposes in IP networks.         ICMP packets are encapsulated within IP packets but do not have the concept of source and destination ports like some other transport layer protocols such as TCP or UDP.
  - b. Below is attached echo request packet. Type is 8 and code is 0 which is highlited.
    `Frame 7: 98 bytes on wire (784 bits), 98 bytes captured (784 bits) on interface enp0s3, id 0
Ethernet II, Src: PcsCompu_62:db:48 (08:00:27:62:db:48), Dst: RealtekU_12:35:02 (52:54:00:12:35:02)
Internet Protocol Version 4, Src: 10.0.2.15, Dst: 128.93.162.83
Internet Control Message Protocol
    Type: 8 (Echo (ping) request)
    Code: 0
    Checksum: 0x6ddf [correct]
    [Checksum Status: Good]
    Identifier (BE): 10790 (0x2a26)
    Identifier (LE): 9770 (0x262a)
    Sequence Number (BE): 1 (0x0001)
    Sequence Number (LE): 256 (0x0100)
    [Response frame: 8]
    Timestamp from icmp data: Jan 30, 2024 04:17:00.000000000 GMT
    [Timestamp from icmp data (relative): 0.608431546 seconds]
    Data (48 bytes)`

  - c. All the fields in ICMP packets are as follows
    - Type (8 bits):
        Use: Identifies the specific type of ICMP message. Different types serve different purposes, such as Echo Request, Echo Reply, Destination Unreachable, Time Exceeded, etc.
    - Code (8 bits):
        Use: Further refines the message type, providing additional information about the ICMP message. For example, for an Echo Request, the code might specify variations of the request.
    - Checksum (16 bits):
        Use: Ensures the integrity of the ICMP packet during transmission. The checksum is computed over the ICMP header and data fields.

    - Identifier (16 bits):
        Use: Typically used in Echo Request and Echo Reply messages to help match requests with their corresponding replies. It allows the sender and receiver to correlate multiple requests and responses.
    - Sequence Number (16 bits):
        Use: Works in conjunction with the Identifier to identify the order of Echo Request and Echo Reply messages. Helps in distinguishing different packets within the same session.
    - Timestamp (32 bits) and Timestamp Reply (32 bits):
        Use: Present in Timestamp and Timestamp Reply messages, used for measuring the round-trip time between the source and destination. The Timestamp field contains the time the Echo Request was sent, and the Timestamp Reply field contains the time the reply was sent.
  - d. Below is attached echo reply packet. Type is 0 and code is 0 which is highlited.
    `Frame 8: 98 bytes on wire (784 bits), 98 bytes captured (784 bits) on interface enp0s3, id 0
Ethernet II, Src: RealtekU_12:35:02 (52:54:00:12:35:02), Dst: PcsCompu_62:db:48 (08:00:27:62:db:48)
Internet Protocol Version 4, Src: 128.93.162.83, Dst: 10.0.2.15
Internet Control Message Protocol
    Type: 0 (Echo (ping) reply)
    Code: 0
    Checksum: 0x75df [correct]
    [Checksum Status: Good]
    Identifier (BE): 10790 (0x2a26)
    Identifier (LE): 9770 (0x262a)
    Sequence Number (BE): 1 (0x0001)
    Sequence Number (LE): 256 (0x0100)
    [Request frame: 7]
    [Response time: 186.840 ms]
    Timestamp from icmp data: Jan 30, 2024 04:17:00.000000000 GMT
    [Timestamp from icmp data (relative): 0.795271068 seconds]
    Data (48 bytes)
`
  - e. Yes ICMP echo request and reply packets have the same fields.As it is visible in the above echo request and echo reply packet, they have same fields.
      In general, ICMP Echo Request and Echo Reply packets have similar fields, but there are some differences related to the specific nature of the request and response.
### Solution 3.
Tracert request and responses to website www.inria.fr are as follows.
  - a.
  - b.
  - c.
