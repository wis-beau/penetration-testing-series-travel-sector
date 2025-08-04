# Recon & Scanning Phase

**Passive Recon:**  
- Google Dorking revealed `.git/config` indexed on public search  
- DNS enumeration found subdomain: `dev.tripplanner.test`

**Active Scanning:**  
- Nmap scan:
  - Port 80 (Main App)
  - Port 8080 (Legacy dev panel)
- Dirb revealed `/admin-dev/` and `/backup.zip`
