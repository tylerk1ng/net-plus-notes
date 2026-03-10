# Layer 5: Session

**Function**: Establishes, manages, and terminates sessions between apps.

**PDU**: Data (adds session header to L6 PDU → segment).

**Key protocols/devices**: NetBIOS, RPC, SQL, checkpoints/dialog control.

**Encapsulation**: Adds session info to L6 data before transport layer.

**Common issues**: "Connection reset"? Session layer dialog control failed.

**Attack example**: Session hijacking

**Professor Messer notes**: 
- "Control layer for tunneling/setup"

**THM notes**: 
- once data is correctly translated or formatted from L6, L5 will create and maintain connection to other computer
- connection established = a session is created
- sessions are unique
- comm mgmt between devices, control & tunneling, protocols
