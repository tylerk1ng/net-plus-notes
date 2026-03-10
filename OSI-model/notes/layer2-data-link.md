# Layer 2: Data Link

**Function**: Node-to-node delivery on same network, error detection, flow control.

**PDU**: Frame—adds data link header/trailer to L3 packet.

**Key protocols/devices**: Ethernet, PPP, ARP (IP to MAC), switches, bridges. MAC addresses.

**Encapsulation**: Wraps L3 packet with Ethernet header (src/dest MAC) + trailer (FCS for errors).

**Common issues**: Duplicate MACs or no switch port light? L2 problem.
**Attack examples**: ARP poisoning/spoofing

**Professor Messer notes**: 
- "MAC addresses, switches, frames—DLC protocols"
- "language", switching, MAC address on Ethernet

**THM notes**: 
- MAC in packet capture tasks
- receives packet from L3
- including IP addy & adds physical MAC addy of receiving endpoint to create a frame
