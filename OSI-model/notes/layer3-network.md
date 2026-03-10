# Layer 3: Network

**Function**: Logical addressing and routing packets across multiple networks.

**PDU**: Packet (or datagram)—adds network header to L4 segment.

**Key protocols/devices**: IP (IPv4/IPv6), ICMP (ping), routers, L3 switches, OSPF/RIP.

**Encapsulation**: Wraps L4 segment with IP header (source/dest IP) → routes to next hop.

**Common issues**: "Destination unreachable"? Wrong subnet or routing table.

**Attack example**: IP spoofing

**Professor Messer notes**: 
- "IP addresses and routers live here"

**THM notes**: 
- routing and re assembly of data
- OSPF = open shortest path first
- RIP = routing information protocol
- everything here dealt with using IP addys
- routing, IP, fragments frames
