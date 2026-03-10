# Layer 6: Presentation

**Function**: Translates data between app format and network format (syntax).

**PDU**: Data (adds presentation header to L7 data).

**Key protocols/devices**: ASCII/Unicode, JPEG/GIF, SSL/TLS handshake, compression.

**Encapsulation**: Wraps L7 data; handles encryption (e.g., HTTPS TLS) before L5.

**Common issues**: Garbled text in email? Presentation layer mismatch.

**Attack example**: SSL stripping

**Professor Messer notes**: 
- "Encryption/decryption happens here, like SSL"

**THM notes**: 
- standardization takes place
- main purpose: translator for data to and from L7
- sec features like data encryption occur at L6

