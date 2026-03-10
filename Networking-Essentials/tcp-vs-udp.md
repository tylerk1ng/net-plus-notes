# TCP vs UDP (Layer 4 Transport - Sec+ Focus)

**Why care?** Firewalls filter by protocol. Sec+ asks: "TCP for file transfer, UDP for DNS?"

## Comparison Table

| Feature          | TCP (Reliable)              | UDP (Fast)                  |
|------------------|-----------------------------|-----------------------------|
| Connection       | 3-way handshake             | Connectionless              |
| Delivery         | Guaranteed (ACKs, retransmit)| Best-effort (no ACKs)       |
| Order            | In-sequence                 | No order guarantee          |
| Speed            | Slower (overhead)           | Faster (minimal header)     |
| Header Size      | 20-60 bytes                 | 8 bytes fixed               |
| Flow Control     | Yes (windowing)             | No                          |
| Error Recovery   | Yes                         | Basic checksum only         |

**Sec+ Use Cases**:
- **TCP**: Web (80/443), SSH (22), RDP (3389), file transfers
- **UDP**: DNS (53), streaming, VoIP, DHCP

**Attack Relevance**:
- TCP: SYN flood (half-open connections)
- UDP: Amplification (DNS/NTP reflection)

**THM Note**: Nmap `-sT` (TCP) vs `-sU` (UDP) scans.
**Messer**: Net+ 1.4 Transport layer.
