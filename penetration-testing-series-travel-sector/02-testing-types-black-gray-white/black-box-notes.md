# Black Box Test Notes

- **Start Point:** login.travelagency.test
- **Tools Used:** Dirb, Burp Suite, Hydra

- **Findings:**
  - Discovered `/admin-login` via forced browsing
  - Password policy allows short/simple passwords (6 chars)
  - No lockout after failed attempts
