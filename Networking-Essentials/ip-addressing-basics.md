# IP Addressing Basics (Sec+ Domain 2.5)

**IPv4 Format**: 4 octets (0-255), dotted decimal. e.g., 192.168.1.100

## Key Concepts

**Subnet Mask**: Defines network vs host portion. Common:
- /24 = 255.255.255.0 (256 IPs, 254 usable)
- /16 = 255.255.0.0 (65k IPs)

**Private Ranges (RFC 1918)**: Non-routable on Internet:
| Range              | CIDR    | Typical Use    |
|--------------------|---------|----------------|
| 10.0.0.0 - 10.255.255.255 | /8   | Large networks |
| 172.16.0.0 - 172.31.255.255 | /12 | Medium nets   |
| 192.168.0.0 - 192.168.255.255 | /16 | Home/small    |

**Special Ranges**:
- 127.0.0.1: Loopback (localhost)
- 169.254.0.0/16: APIPA (auto when DHCP fails)
- 0.0.0.0/0: Default route ("all networks")

**NAT/PAT**: Private IPs → public (router overloads port 1024-65535). Hides internal network.

**Sec+ Relevance**:
- Segmentation: VLANs/subnets limit breach spread
- Attacks: IP spoofing (fake source IP)

**THM**: Network Fundamentals rooms.
**Messer**: Net+ 1.3 IP Addressing.
