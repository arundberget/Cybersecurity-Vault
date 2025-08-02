# Reconnaissance Tools

Reconnaissance tools enable attackers and security professionals alike to gather critical information about a target. These tools can automate passive discovery or actively probe a system for publicly available intelligence before any exploitation begins.

Many of these tools are also referenced in [[docs/04_Scanning/Tools|scanning phases]] but are used differently during recon, often with stealth in mind.

---

## Categories of Reconnaissance Tools

### DNS and WHOIS Lookup Tools

These provide basic domain-level metadata and infrastructure information.

- **whois.domaintools.com** - Domain registration details
- **dig**, **nslookup** - DNS record queries
- **Shodan** - Internet-connected device and service search engine
- **Censys** - Similar to Shodan, with focus on certificates and infrastructure visability

These tools help identify organizational structure, hosting providers, and external services.

---

### Web and Social Reconnaissance Tools

Useful for finding surface-level information on people, systems, or organizations.

- **Google Dorking** – Targeted search operators for exposed content  
- **theHarvester** – Email and subdomain enumeration from public sources  
- **Maltego** – Link analysis of people, infrastructure, and entities  
- **SpiderFoot** – Comprehensive OSINT automation (subdomains, leaks, etc.)  
- **Recon-ng** – Reconnaissance framework with modular functionality for footprinting

---

### Email and Credential Hunting

- **Have I Been Pwned** – Checks for leaked credentials  
- **Hunter.io** – Email pattern and address discovery  
- **LeakLooker / BreachDirectory** – Search past data breaches for target identities

---

### Metadata Extraction

- **ExifTool** – Pulls metadata from documents, images, etc.  
- **FOCA** – Extracts metadata and hidden data from documents found via web crawlers

This is helpful for identifying internal usernames, software used, or timestamp leakage.

---

### Visualization and Enumeration

- **Maltego** – Repeated here for visual mapping  
- **Zenmap** – Graphical frontend for Nmap, sometimes used for visualizing scan results  
- **dnsenum**, **dnsrecon** – DNS zone transfer and enumeration tools  

---

## Tool Selection Considerations

- **Passive vs. Active** – Does it interact with the target?  
- **Detection Risk** – Passive tools are stealthier  
- **OSINT Depth** – Tools like SpiderFoot and theHarvester cover many vectors  
- **Integration** – Frameworks like Recon-ng allow chaining and automation  

---

## Notes

- Reconnaissance tools are often used during both **initial engagement planning** and **scanning prep**  
- Outputs from tools like theHarvester can directly feed into [[Target_Selection|target profiling]]  
- Many tools are built into platforms like Kali Linux and Parrot OS

---

#recon #tools #osint #footprinting #preattack

---

_Last updated: August 1, 2025_