# OSI Model

The OSI (Open Systems Interconnection) Model is a conceptual framework used to describe how different networking functions interact across a network. It consists of seven layers, each with specific responsibilities.

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

### Layer 1: Physical
- Concerned with physical media: cables, voltages, connectors
- Examples, Ethernet cables, radio waves, fiber optics

### Layer 2: Data Link
- Responsible for reliable link-to-link communication
- Uses MAC addresses, handles framing and error detection
- Examples: Ethernet, ARP, PPP

### Layer 3: Network
- Handles logical addressing and routing between networks
- Works with IP addresses and subnets
- Examples: IP, ICMP, IPSec

### Layer 4: Transport
- Provides end-to-end delivery between systems
- Manages flow control, sequencing, error recovery
- Examples: TCP (reliable), UDP (faster, connectionless)

### Layer 5: Session
- Manages and controls the dialog between applications
- Keeps sessions alive, syncs communication
- Examples: RPC, NetBIOS

### Layer 6: Presentation
- Translates data between applications and the network
- Handles encryption, compression, and data formatting
- Examples: TLS, SSL, Base64, JPEG

### Layer 7: Application
- Closest to the end user
- Provides services like email, file transfer, and web browsing
- Examples: HTTP, FTP, DNS, SMTP