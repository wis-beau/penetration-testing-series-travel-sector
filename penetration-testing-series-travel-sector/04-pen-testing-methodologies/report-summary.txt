# Pen Test Summary – EasyFly App (PTES Aligned)

**Methodology:** PTES  
**Scope:** Mobile app and backend APIs  
**Findings:**
- Dev API left publicly exposed  
- Admin login bypassed via test credentials  
- Lack of MFA or token expiration

**Risk:** High – potential unauthorized access to flight engine

**Remediation:**  
- Remove dev endpoints before production  
- Enforce token expiration + MFA  
- Set rate limits and IP monitoring
