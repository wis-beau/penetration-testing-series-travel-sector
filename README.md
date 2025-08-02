# 🛡️ TripPlanner Penetration Testing Case Study

This repository documents a simulated grey-box penetration test against a fictional travel platform, **TripPlanner Ltd**, as part of an educational project on ethical hacking.

---

## 📁 Repository Structure
├── reports/
│ ├── tripplanner-penetration-summary.pdf # Executive summary report
│ └── tripplanner-raw-findings.md # Raw technical findings
│
├── usage-demos/
│ ├── reconnaissance/
│ │ ├── nmap-tripplanner.md
│ │ ├── theharvester-tripplanner.md
│ │
│ ├── scanning/
│ │ ├── nikto-tripplanner.md
│ │ ├── sslscan-tripplanner.md
│ │
│ ├── gaining-access/
│ │ ├── hydra-tripplanner.md
│ │ ├── sqlmap-tripplanner.md
│ │
│ ├── maintaining-access/
│ │ └── metasploit-tripplanner.md
│ │
│ ├── privilege-escalation/
│ │ └── linpeas-tripplanner.md
│ │
│ ├── reporting/
│ │ ├── dradis-reporting.md
│ │ └── cherrytree-tripplanner.ctd
│
├── notes/
│ └── cherry-notes-export.ctd # Internal note exports

---

## 🧭 Case Summary

- **Test Target:** `tripplanner.io` (Fictional Travel Booking Platform)
- **Test Window:** 24–28 July 2025
- **Test Type:** Grey Box  
- **Team:** SageSecOps – Red Team Lab

---

## 🔍 Key Techniques & Tools Used

| Phase                   | Tools Used                                |
|------------------------|--------------------------------------------|
| Reconnaissance         | Nmap, theHarvester, WHOIS                 |
| Scanning               | Nikto, SSLScan, WPScan                    |
| Gaining Access         | Hydra, SQLMap, Burp Suite                 |
| Maintaining Access     | Metasploit, Reverse Shells                |
| Privilege Escalation   | LinPEAS, Cron Exploits                    |
| Reporting              | CherryTree, Dradis, Markdown              |

---

## 📷 Visual Map (Optional)

![TripPlanner Tool Stack](./assets/tripplanner-tool-stack.png)

---

## 📎 Disclaimer

This case study is for **educational purposes only** and does not target any real-world systems. All domains and infrastructure are fictional.

---

## 📬 Feedback & Contributions

Open an issue or submit a pull request if you want to improve this repo or adapt it to your own learning path.


