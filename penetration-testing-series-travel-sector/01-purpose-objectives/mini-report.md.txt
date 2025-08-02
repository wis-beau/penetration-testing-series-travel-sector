# Mini Penetration Test Report – Hotel Booking Platform

**Client:** BoutiqueStay Hotels  
**Scope:** Online Booking Application  
**Test Type:** Black Box  
**Test Date:** 2025-07-28

---

## 🧾 Summary

During a scoped and authorized test, our team discovered a critical SQL injection vulnerability in the promotional code feature of the online booking platform. Exploiting this allowed full read access to the backend bookings database.

---

## 🐛 Findings

- **Vulnerability Type:** SQL Injection  
- **Location:** GET parameter `code` in booking URL  
- **Impact:** Unauthorized access to bookings, customer emails, and internal pricing  

---

## 🔧 Recommendations

- Use prepared statements to prevent SQL injection  
- Implement server-side validation of input  
- Log abnormal query patterns for detection  
- Schedule code reviews focusing on security best practices  

---

## ✅ Status

The vulnerability has been patched. No customer data was accessed beyond the test scope. System monitoring has been activated.

---


