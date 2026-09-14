#OSI Model

The **OSI (Open Systems Interconnection) Model** is a conceptual framework used to understand how data travels across a network.

## OSI Layers (Top to Bottom)

| Layer | Name |
|---------|---------|
| 7 | Application |
| 6 | Presentation |
| 5 | Session |
| 4 | Transport |
| 3 | Network |
| 2 | Data Link |
| 1 | Physical |

---

## Layer 7 - Application

**Examples:**
- HTTP
- DNS
- SMTP
- FTP

This is where **application-level network protocols** operate and interact with end-user applications.

---

## Layer 6 - Presentation

Conceptually concerned with:

- Encoding
- Data representation
- Compression
- Encryption and transformations

> Focus on understanding the purpose rather than memorizing every example.

---

## Layer 5 - Session

Responsible for managing communication sessions between devices.

Examples of responsibilities:

- Session establishment
- Session maintenance
- Session termination

> Do not spend too much time memorizing theoretical examples at this stage.

---

## Layer 4 - Transport

**Most Important Protocols:**
- TCP (Transmission Control Protocol)
- UDP (User Datagram Protocol)

Responsibilities:

- End-to-end communication
- Reliability and error handling
- Flow control
- Segmentation and reassembly

**Ports are associated with this layer.**

---

## Layer 3 - Network

**Most Important Protocols:**
- IP (Internet Protocol)
- ICMP (Internet Control Message Protocol)

Responsibilities:

- Logical addressing
- Routing packets between networks
- Path selection

> Routing happens at Layer 3.

---

## Layer 2 - Data Link

**Examples:**
- Ethernet
- Wi-Fi (802.11)
- MAC Addresses
- ARP-related local network behavior

Responsibilities:

- Local network communication
- Frame delivery
- Physical addressing using MAC addresses

---

## Layer 1 - Physical

The actual transmission medium used to send data.

**Examples:**
- Copper Cables
- Radio Waves
- Electrical Signals
- Fiber Optic Cables

Responsibilities:

- Bit transmission
- Signal generation
- Physical connectivity

---

## Quick Memory Trick
