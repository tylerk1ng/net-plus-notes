# Layer 7: Application

**Function**: Provides network services directly to user apps and end-user processes.

**PDU**: Data (no header added here—starts encapsulation).

**Key protocols/devices**: HTTP/HTTPS, FTP, SMTP, DNS, POP3/IMAP, DHCP client.

**Encapsulation**: Generates raw application data that L6 wraps with presentation header.

**Common issues**: Browser can't load site? Check DNS (L7) before lower layers.

**Attack examples**: phising, SQLi

**Professor Messer notes**: 
- "Layer where we interact with apps like web browsers"

**THM notes**: 
- we see this layer
- email clients, web browsers, FileZilla
- they provide a friendly Graphical User Interface (GUI)

