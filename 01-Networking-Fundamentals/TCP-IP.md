# TCP/IP Model

In the real world, you'll frequently encounter the **TCP/IP Model** rather than the OSI model.

The TCP/IP model is a more practical networking model used throughout the Internet and modern networks, while the OSI model is primarily used as a conceptual learning framework.

## TCP/IP Layers

| Layer | Purpose |
|---------|---------|
| Application | Provides network services to applications |
| Transport | End-to-end communication between devices |
| Internet | Logical addressing and routing |
| Network Access | Physical network communication |

---

## Layer 4 - Application

This layer combines the functionality of the top three OSI layers:

- Application
- Presentation
- Session

**Common Protocols:**

- HTTP
- HTTPS
- DNS
- SMTP
- POP3
- IMAP
- FTP
- SSH

This is where applications communicate over the network.

---

## Layer 3 - Transport

Responsible for communication between endpoints.

**Main Protocols:**

- TCP (Transmission Control Protocol)
- UDP (User Datagram Protocol)

### TCP
- Reliable
- Connection-oriented
- Error checking
- Packet retransmission

Examples:
- Web browsing (HTTP/HTTPS)
- Email
- File transfers

### UDP
- Faster
- Connectionless
- No delivery guarantee

Examples:
- Streaming
- VoIP
- Online gaming
- DNS queries

> Ports operate at the Transport Layer.

---

## Layer 2 - Internet

Responsible for logical addressing and routing traffic between networks.

**Main Protocols:**

- IP (Internet Protocol)
- ICMP (Internet Control Message Protocol)

Responsibilities:

- Packet routing
- Addressing
- Path selection

Examples:

- IPv4
- IPv6
- Ping (ICMP)

> Routers primarily operate at this layer.

---

## Layer 1 - Network Access

Responsible for transmitting data across the local network and physical medium.

**Examples:**

- Ethernet
- Wi-Fi
- MAC Addresses
- Fiber Optic Cables
- Copper Cables
- Radio Signals

Responsibilities:

- Physical transmission
- Frame delivery
- Hardware communication

> This layer combines OSI Layers 1 and 2.

---

# OSI to TCP/IP Mapping

| OSI Model | TCP/IP Model |
|------------|-------------|
| Layer 7 - Application | Application |
| Layer 6 - Presentation | Application |
| Layer 5 - Session | Application |
| Layer 4 - Transport | Transport |
| Layer 3 - Network | Internet |
| Layer 2 - Data Link | Network Access |
| Layer 1 - Physical | Network Access |

---

## Visual Mapping

```text
OSI Model                      TCP/IP Model

7 Application      ┐
6 Presentation     ├──► Application
5 Session          ┘

4 Transport        ───► Transport

3 Network          ───► Internet

2 Data Link        ┐
1 Physical         ┘──► Network Access
```

---

## Quick Exam Tip

### OSI Model (7 Layers)

```text
Application
Presentation
Session
Transport
Network
Data Link
Physical
```

### TCP/IP Model (4 Layers)

```text
Application
Transport
Internet
Network Access
```

---

## Key Takeaway

- **OSI Model** = Learning and troubleshooting framework
- **TCP/IP Model** = Real-world networking model
- **TCP/IP is simpler**, combining multiple OSI layers into four practical layers
- Most networking discussions focus on:
  - HTTP/HTTPS (Application)
  - TCP/UDP (Transport)
  - IP (Internet)
  - Ethernet/Wi-Fi (Network Access)

> For networking and cybersecurity, understand how **HTTP → TCP → IP → Ethernet/Wi-Fi** work together, as this represents the path data takes through the TCP/IP model.
