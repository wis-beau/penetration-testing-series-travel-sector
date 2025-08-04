# Execution Notes by PTES Phase

**Intelligence Gathering**  
- Identified `/api/test/dev_login` via mobile traffic inspection

**Vulnerability Analysis**  
- Endpoint accepts plaintext login with no rate limit

**Exploitation**  
- Gained unauthorized admin token  
- Modified flight pricing data

**Post-Exploitation**  
- Created alerts on token usage for devs to monitor future attacks
