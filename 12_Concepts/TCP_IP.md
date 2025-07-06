# TCP/IP Model

The TCP/IP (Transmission Control Protocol/Internet Protocol) model is a four-layer framework that defines how data is transmitted over the internet. It serves as the **real-world implementation** of networking functions, compared to the more academic [[OSI_Model|OSI model]].

---

## Layer Comparison

| TCP/IP Layer   | Corresponding OSI Layer                        | Function                          | Example                  |
| -------------- | ---------------------------------------------- | --------------------------------- | ------------------------ |
| Application    | 7 - Application, 6 - Presentation, 5 - Session | Interface for user and apps       | HTTP, FTP, DNS, SMTP     |
| Transport      | 4 - Transport                                  | End-to-end delivery, segmentation | TCP, UDP                 |
| Internet       | 3 - Network                                    | Routing and logical addressing    | IP, ICMP, IPSec          |
| Network Access | 2 - Data Link, 1 - Physical                    | Physical delivery over media      | Ethernet, ARP, PPP, WiFi |

While the OSI model separates concepts into seven layers, TCP/IP simplifies them into four **operational layers**, each implemented in real-world devices and software.

---

## Layer Details

### Network Access Layer
This layer corresponds to the bottom of the OSI stack and includes both physical and data link layer tasks.

- Interfaces with physical hardware
- Manages MAC addressing and frame transmission
- Supports Ethernet, PPP, and wireless protocols
- Tools like [[Wireshark]] can inspect this layer
### Internet Layer
Manages packet forwarding and addressing using IP addresses. It determines **how data gets from source to destination**.

- Protocols: IP, ICMP, ARP, IPSec
- Vulnerable to attacks like spoofing and scanning (see [[Scanning_Considerations|scanning considerations]])

### Transport Layer
Ensures data is delivered reliably or quickly between hosts.

- TCP provides reliable, ordered delivery
- UDP offers faster, connectionless communication
- TCP port numbers tie directly into [[Port_Scanning|port scanning]] and service enumeration.

### Application Layer
Provides protocols used by programs like web browsers, email clients, and file transfer tools.

- Protocols: HTTP, DNS, SMTP, FTP
- Layer most visible to users and attackers
- Needs [[Web_Application_Security|web application security]] and session handling to counter threat actors

---

## Notes

- TCP/IP is flexible and modern — protocols like [[TLS]] and [[HTTPv2|HTTP/2]] sit at the Application Layer.
- Layer boundaries are less strict in TCP/IP than in OSI.

## Embedded Tools and Relevance

- Tools like [[08_Red_Team_Tools/Nmap]] and [[Wireshark]] rely on understanding of TCP/IP to capture, analyze, and simulate network traffic.
- Knowing this model is essential for both the [[PenTest_Processes|penetration test processes]] and [[Incident_Response|incident response]].

---

#tags 
#concept/networking #tcpip #foundation #reference

---

_Updated July 4, 2025_