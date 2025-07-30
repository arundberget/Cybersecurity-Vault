# Target Selection

Target selection is the strategic process of identifying which systems, users, or applications will be evaluated during a penetration test. This occurs early in the engagement and directly shapes how the assessment will be conducted.

The process must align with business priorities, known risks, and the legally defined [[Engagement_Contracts|engagement contracts]]. Proper target selection also ensures that [[PenTest_Processes|penetration testing]] efforts are efficient, ethical, and in-scope.

---

## Selection Considerations

### Asset Value

Testers prioritize systems that store, process, or transmit sensitive data. These may include:

- Customer records
- Payment systems
- Intellectual property
- Authentication services (e.g., Active Directory)

Assets are often ranked using business impact analysis or risk classification systems.

### Exposure and Accessibility

Externally facing services are typically assessed first, as they're accessible to threat actors without internal access.

- Web servers
- VPN endpoints
- Mail servers
- APIs

Internal systems may be selected later in the engagement or during internal test scenarios.

### Risk Profile

Organizations may target:

- Systems with known vulnerabilities
- Legacy infrastructure
- Critical services with high availability requirements

This aligns closely with the threat modeling phase, where likely attack paths and [[Threat_Actors|threat actors]] are considered.

---

## Types of Targets

| Target Type         | Description                                                                          |
| ------------------- | ------------------------------------------------------------------------------------ |
| IP Ranges           | Common in network tests (internal/external)                                          |
| Web Applications    | Assessed for authentication, input handling, and data access flaws                   |
| Mobile Applications | Tested for insecure storage, traffic interception, and misuse of permissions         |
| User Roles          | Role-based testing evaluates privilege escalation, data access, and session security |
| Physical Systems    | Badge systems, security cameras, or on-prem servers for physical access tests        |

---

## Prioritization Strategy

Effective target selection includes:

- **High-impact first**: Focus on systems where compromise would cause the most damage
- **Easily reachable**: Test systems exposed to the internet or connected networks
- **Client-identified targets**: Organizations may request tests on specific services or systems

This prioritization helps maximize value while staying aligned with client expectations and contract scope.

---

## Notes

- Target selection must be documented before scanning or exploitation begins
- All targets should be pre-approved in writing as part of the engagement agreement
- Selection may evolve if critical systems are discovered during reconnaissance (with client approval)

---

#tags 
#preattack #targeting #scope #risk #planning

---

_Last updated: July 29, 2025_