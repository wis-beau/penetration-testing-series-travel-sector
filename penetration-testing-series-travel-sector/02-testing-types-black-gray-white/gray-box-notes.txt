# Gray Box Test Notes

- **Credentials Provided:** user_demo / Travel@123
- **Tools Used:** Burp Suite, Browser DevTools

- **Findings:**
  - `GET /user?uid=111` → shows own data
  - `GET /user?uid=112` → reveals another user's booking
  - No access control on user ID
  - Called an Insecure Direct Object Reference (IDOR)
