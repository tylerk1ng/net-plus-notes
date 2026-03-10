# OSI Model Overview (Top to Bottom)

**Data flow**: Starts at Application (L7), gets encapsulated down to Physical (L1), transmits, then decapsulated up at receiver.

**Encapsulation**: Process where each layer wraps the data from the layer above it with its own header. This adds addressing, error checking, and protocol info so devices know how to handle the data. Reverse process (decapsulation) strips headers as data moves up layers at destination. 

**Example**: Web request starts as HTTP data (L7) → TCP header added (L4) → IP header (L3) → Ethernet frame (L2) → bits on wire (L1).

**7 Layers** :  
- **Layer 7: Application** – User apps and services (HTTP, FTP, DNS, POP3).  
- **Layer 6: Presentation** – Data formatting, encryption, compression (JPEG, SSL).  
- **Layer 5: Session** – Manages connections, checkpoints, sync (NetBIOS, RPC).  
- **Layer 4: Transport** – End-to-end delivery, ports (TCP, UDP).  
- **Layer 3: Network** – Logical addressing, routing (IP, routers).  
- **Layer 2: Data Link** – Frames, MAC addresses (Ethernet, switches).  
- **Layer 1: Physical** – Bits, cables, signals (RJ45, hubs). 

**Mnemonic** (top-down): All People Seem To Need Data Processing.

**Study notes**: 
- Encapsulation = wrapping data like Russian dolls
- Encapsulation = when pieces of information get added to data
- Each layer only sees data from layer above/below
