# Threat Actors

Threat actors are individuals or groups that intentionally cause harm or disruption to an organization's systems, networks, or data. Understanding thread actor types is essential for anticipating potential attacks, evaluating risk, and developing proactive security strategies.

Threat modeling often begins with identifying who your adversaries are, a critical step before conducting any technical testing or assessments.

---

## Categories or Threat Actors

### Script Kiddies

Script kiddies are unskilled attackers who use pre-written tools or scripts without a deep understanding of how they work.

- Motivated by curiosity, boredom, or clout
- Typically target low-hanging fruit
- Easily deterred by basic security controls
### Hacktivists

Hacktivists are politically or socially motivated attackers.

- Goal is often disruption, defacement, or publicity.
- Targets may include governments, corporations, or controversial figures
- Tactics include DDoS, defacements, or information leaks

### Organized Crime

These groups operate like businesses, driven by profit.

- Run large-scale operations like ransomware, data theft, or card skimming
- Use sophisticated tools, phishing campaigns, and remote access Trojans
- Often operate from outside the victim's legal jurisdiction

### Insider Threats

Insiders have authorized access to systems and data.

- May be employees, contractors, or third parties
- Can be malicious (disgruntled employee) or unintentional (negligent behavior)
- Difficult to detect using traditional perimeter-based security

### State-Sponsored Actors (Nation-States)

Highly skilled and well-funded, these actors pursue national or strategic goals.

- Often target critical infrastructure, intellectual property, or political systems
- Use custom malware, zero-day exploits, and long-term persistence
- May overlap with advanced persistent threat (APT) groups

### Competitors

Although less common, some threat actors may come from rival organizations attempting to gain business or strategic advantage.

- Illegal in most jurisdictions
- May involve espionage, surveillance, or sabotage

---

## Key Characteristics

| Actor Type      | Motivation            | Capability | Example Tactics               |
| --------------- | --------------------- | ---------- | ----------------------------- |
| Script Kiddies  | Curiosity / Malicious | Low        | Scanning, tool-based exploits |
| Hacktivists     | Ideology              | Medium     | DDoS, defacement              |
| Organized Crime | Profit                | High       | Ransomware, phishing          |
| Insiders        | Varies                | Medium     | Misuse of privileges          |
| Nation-States   | Political             | Very High  | APTs, zero-days, stealth ops  |
| Competitors     | Strategic             | Medium     | Espionage, surveillance       |

---

## Threat Actor Relevance in Security Work

Identifying the likely threat actors for an environment informs:

- Risk scoring and prioritization in assessments
- What data or systems are most at risk
- Which tools, techniques, and procedures to simulate during the [[PenTest_Processes|penetration test process]]
- Legal and contractual obligations outlined in [[Engagement_Contracts|engagement contracts]]

---

## Notes

- Some actors evolve over time - script kiddies may become part of organized groups
- Attribution is difficult; attackers may hide their identity or operate through proxies
- Defenders must consider both external and internal threats when modeling risk

---

#tags 
#preattack #threatactors #risk #pentest #profiling

---

_Last updated: July 29, 2025_