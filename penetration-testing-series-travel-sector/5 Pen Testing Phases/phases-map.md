# 🗂️ Penetration Testing Phases – Mapping to PTES & OWASP

This table maps each phase of the TripPlanner penetration test to relevant sections from:

- PTES – Penetration Testing Execution Standard
- OWASP Web Security Testing Guide (WSTG)

| Phase | PTES Reference | OWASP WSTG Section(s) | TripPlanner Example |
|-------|----------------|-----------------------|---------------------|
| 1. Pre-Engagement & Scoping | Pre-Engagement Interactions | N/A | Rules of Engagement, scope definition, authorization |
| 2. Reconnaissance & Scanning | Intelligence Gathering | WSTG-INFO-01, WSTG-INFO-02 | Whois lookup, subdomain enumeration, tech stack fingerprinting |
| 3. Threat Modeling | Threat Modeling | N/A | Prioritized CMS & API testing based on risk |
| 4. Vulnerability Identification | Vulnerability Analysis | WSTG-INPV-01, WSTG-INPV-05, WSTG-ATHN-02 | File upload bypass, SQL Injection, verbose API errors |
| 5. Exploitation | Exploitation | Relevant OWASP category per vuln | Web shell upload, SQLi auth bypass |
| 6. Post-Exploitation | Post-Exploitation | N/A | Privilege escalation via cron job, persistence testing |
| 7. Reporting | Reporting | N/A | Summary & technical report delivered |

---
