# 🧭 Methodology Mapping – TripPlanner Penetration Test

This table maps key test activities from the TripPlanner engagement to corresponding sections from two widely recognized penetration testing frameworks:

- **OWASP Web Security Testing Guide (WSTG)**
- **PTES – Penetration Testing Execution Standard**

| Test Activity                          | OWASP WSTG Section              | PTES Phase                    |
|----------------------------------------|----------------------------------|-------------------------------|
| Scoping and Rules of Engagement        | N/A                              | Pre-engagement Interactions   |
| Reconnaissance (whois, subdomain enum) | WSTG-INFO-01, WSTG-INFO-02       | Intelligence Gathering        |
| Port scanning & service fingerprinting | WSTG-INF-01, INF-02              | Threat Modeling               |
| CMS file upload test                   | WSTG-CLNT-05, WSTG-INPV-01       | Vulnerability Identification  |
| SQL Injection (Login form)             | WSTG-INPV-05, WSTG-ATHN-02       | Vulnerability Identification  |
| Brute force (Hydra – login endpoint)   | WSTG-ATHN-07                     | Vulnerability Identification  |
| Privilege escalation via cron job      | WSTG-BUSL-01, WSTG-APIT-02       | Exploitation                  |
| Risk analysis + reporting              | N/A                              | Post-Exploitation & Reporting |

---

## 📝 Notes

- Testing activities align with a **hybrid methodology**, combining the structure of PTES with OWASP’s web-focused technical depth.
- Activities not directly mapped in OWASP (e.g., pre-engagement) are handled by PTES phases.
- Methodology was adapted based on scope, access level, and TripPlanner’s application stack.

---

