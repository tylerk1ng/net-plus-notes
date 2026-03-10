# Wireless Security (Sec+ Domain 4.1)

**Goal**: Secure WiFi against rogue APs, cracking.

## Protocols Table

| Protocol | Strength                  | Weakness              |
|----------|---------------------------|-----------------------|
| WEP      | Deprecated                | Cracked in minutes   |
| WPA2-PSK | TKIP/AES (handshake vuln) | KRACK, dict attacks  |
| WPA3     | SAE handshake, PMF        | Transition mode risks|
| WPA3-Ent | 802.1X RADIUS auth        | Best for enterprise  |

**Common Attacks**:
- **Evil Twin**: Fake AP steals creds (deauth → captive portal)
- **Rogue AP**: Unauthorized AP on network (employee hotspot)
- **Deauth Flood**: DoS (WPA3 PMF resists)

**Mitigations**:
- WPA3 + disable legacy (WPA/WPA2)
- 802.1X certs, disable WPS
- Wireless IPS scans rogues

**THM**: WiFi Hacking rooms.
**Messer**: SY0-701 4.1 Wireless Settings.
