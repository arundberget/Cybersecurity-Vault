# OSI Model

The OSI (Open Systems Interconnection) Model is a conceptual framework used to describe how different networking functions interact across a network. It consists of seven layers, each with specific responsibilities and aligns closely with concepts found in the [[TCP_IP|TCP/IP]] model.

---

## Layer Summary

| Layer | Name | Function | Example Protocols |
| ----- | ----- | ----- | ----- |
| 7 | Application | End-user access, network services | HTTP, FTP, DNS, SMTP |
| 6 | Presentation | Data format, encryption, compression | TLS, JPEG, ASCII, SSL |
| 5 | Session | Connection management | NetBIOS, RPC, PPTP |
| 4 | Transport | Reliable delivery, segmentation | TCP, UDP |
| 3 | Network | Routing and logical addressing | IP, ICMP, IPSec |
| 2 | Data Link | MAC addressing, frame transmission | Ethernet, ARP, PPP, VLAN |
| 1 | Physical | Electrical/physical transmission | Cables, Hubs, Wi-fi, Fiber |

---

## Layer Details

The OSI Model breaks down communication into **layers**, helping network engineers and cybersecurity professional isolate problems and threats more effectively.

### Layer 1: Physical
Responsible for the raw transmission of bits over a medium. Common attack types here include hardware taps and [[Physical_Security|physical intrusion]].

### Layer 2: Data Link
This layer handles MAC addressing and local network communication. Tools like [[Wireshark]] operate at this and higher layers, revealing frame-level traffic.

### Layer 3: Network
This layer works with IP addresses and routing. Protocols like IP and ICMP are commonly exploited in reconnaissance (see: [[Scanning_Process|Scanning Process]] and [[Reconnaissance_Tools|Reconnaissance Tools]]).

### Layer 4: Transport
Handles connection reliability. Protocols like TCP and UDP are often the targets of [[Port_Scanning|port scanning]] and flooding attacks using tools like [[Nmap]].

### Layer 5: Session
This layer establishes, manages, and terminates communication sessions. Session hijacking is a common attack technique.

### Layer 6: Presentation
This layer ensures data is in a usable format and handles encryption and decryption. It connects directly to concepts found in [[Encryption|encryption]] and [[SSL_TLS|SSL/TLS]].

### Layer 7: Application
The interface for user-level applications like web browsers or email clients. Common attacks here include XSS and injection attacks, often seen in [[Web_Application_Security|web application security]].

---

## Security Relevance by Layer

| Layer | Common Security Risks            |
| ----- | -------------------------------- |
| 7     | Web attacks: XSS, SQL injection  |
| 6     | Weak or outdated encryption      |
| 5     | Session hijacking                |
| 4     | Port scanning, TCP flooding      |
| 3     | IP spoofing, route injection     |
| 2     | MAC spoofing, ARP poisoning      |
| 1     | Hardware taps, physical breaches |

Understanding the OSI Model is essential for both attack and defensive perspectives, especially when applying frameworks like [[MITRE_ATT&CK|MITRE ATT&CK]].

---

## Notes

- All cyber attacks map to one or more OSI layers.
- Many security tools, like [[Wireshark]], [[Nmap]], and [[Zeek]], function across multiple layers.
- The OSI Model is theoretical; the [[TCP_IP|TCP/IP]] model is more commonly implemented in practice.
- You may also want to understand the [[OSI_vs_TCP_Model|difference between the OSI and the TCP Model]]

---

_Updated July 4, 2025_