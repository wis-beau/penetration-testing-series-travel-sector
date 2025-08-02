# Scope Violation Report

## Incident

- On Aug 7, a new intern scanned the live booking API (`prod.tripplanner.com`)
- Scan triggered automated WAF defense → API went offline for 3 mins

## Root Cause

- Misunderstanding of test environment IP range  
- Intern was not briefed on scope boundaries

## Impact

- 3 minutes downtime  
- 11 failed customer bookings  
- Escalation to SecOps and Customer Support

## Resolution

- Added IP filtering to limit tests to staging IPs  
- Conducted emergency briefing for all testers
