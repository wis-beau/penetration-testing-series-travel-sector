# Purpose & Objectives of Penetration Testing – Travel & Tourism Case

## 🎯 Objective
This case study introduces the purpose of penetration testing in the travel and tourism sector. It illustrates how ethical hacking identifies security flaws that could expose sensitive customer data, damage brand reputation, or disrupt business operations.

## 🏨 Case Study: Vulnerable Hotel Booking System

A small hotel chain launched a simple online booking platform. During a routine penetration test, the tester discovered that the **promo code input field** failed to sanitize user input — allowing for a classic SQL injection.

### 🐛 Vulnerability
The tester submitted a common payload:
```sql
' OR '1'='1

This triggered the database to return all bookings, including guest details and staff logins.

✅ Outcome
The vulnerability was disclosed in a safe, legal, and authorized manner.

The development team patched the code using prepared statements.

Logging and input validation were implemented.


Staff were trained on secure coding practices.
