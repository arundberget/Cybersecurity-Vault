# OSI vs TCP/IP Model

The OSI and TCP/IP models both describe how network communication works, but they differ in structure, purpose, and real-world usage.

---

## Comparison Table

| Aspect             | OSI Model (7 Layers)                 | TCP/IP Model (4 Layers)              |
|--------------------|--------------------------------------|--------------------------------------|
| Purpose            | Theoretical reference model          | Practical implementation model       |
| Layers             | 7 (Application to Physical)          | 4 (Application to Network Access)    |
| Layer Separation   | Strict and detailed                  | More abstract and practical          |
| Adoption           | Used for teaching and analysis       | Used in real-world networking        |
| Session Layer      | Exists independently                 | Merged into Application Layer        |
| Presentation Layer | Handles encoding/encryption          | Handled at Application Layer         |
| Transport Layer    | TCP/UDP                              | TCP/UDP                              |
| Network Layer      | IP, ICMP                             | IP, ICMP                             |
| Lower Layers       | Physical/Data Link separated         | Merged as Network Access             |
| Security Mapping   | Clear layer-based threat model       | Used in actual protocol attack chains|

---

## Summary

- The OSI model is primarily used as a **teaching tool** and for **threat modeling**.
- The TCP/IP model is the **de facto standard** used on real networks.
- Cybersecurity professionals must understand **both** models, especially when analyzing tools like [[Wireshark]] or protocols like [[TLS]].

For a deeper breakdown of each model, see:
- [[TCP_IP|TCP/IP]]
- [[OSI_Model|OSI Model]]

---

#tags
#concept/networking #comparison #foundation #reference
