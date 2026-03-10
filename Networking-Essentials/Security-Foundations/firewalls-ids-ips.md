# Firewalls, IDS, IPS (Sec+ Domain 3.2)

**Firewalls**: Block/allow traffic by rules (ports, IP, protocol).

## Types Table

| Type     | Description                          | Example Use |
|----------|--------------------------------------|-------------|
| Packet Filtering | IP/port/state (basic/fast)          | Edge router |
| Stateful | Tracks connections (TCP sessions)   | Corporate FW|
| Proxy    | Intermediates requests (caches)     | Web proxy  |
| NGFW     | App awareness + IPS + URL filtering | Modern UTM |
| WAF      | Web app protection (SQLi, XSS)      | Web server |

**IDS vs IPS**:
- **IDS**: Passive—detects/alerts (logs scans, NIDS on SPAN port)
- **IPS**: Active—blocks inline (drops SYN flood)

**THM**: Splunk IDS labs.
**Messer**: SY0-701 3.2 Firewall Types.
