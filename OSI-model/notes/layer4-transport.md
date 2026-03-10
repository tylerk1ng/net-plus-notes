# Layer 4: Transport

**Function**: End-to-end delivery, error recovery, flow control.

**PDU**: Segment (TCP) or Datagram (UDP)—adds transport header.

**Key protocols/devices**: TCP (reliable), UDP (fast), ports (1024-65535).

**Encapsulation**: Wraps L5 data with TCP/UDP header + port numbers → sends to L3.

**Common issues**: High latency? TCP windowing/flow control.

**Attack example**: SYN flood

**Professor Messer notes**: 
- "Post office layer: TCP/UDP + ports"
  
**THM notes**: 
- Ports in scanning tasks
- when data is sent it follows TCP or UDP
- 3 way handshake: SYN, SYN-ACK, ACK
- connection only est after all 3 steps
- TCP eg. fileshare, email, internet browsing
- UDP eg. video streaming, gaming, ARP & DHCP
