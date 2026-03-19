 Web Application Security: Attack & Defend (PrestaShop)

 Project Overview
This project demonstrates the implementation of a Web Application Firewall (WAF) to protect an e-commerce platform (PrestaShop 8.1.0). The project covers the full lifecycle of a security audit: deployment, hardening, exploitation (XSS), and mitigation.

 Objectives
* Perform administrative account recovery and database hardening via MySQL CLI.
* Simulate a Reflected Cross-Site Scripting (XSS) attack.
* Configure and validate ModSecurity WAF rules to intercept malicious payloads.

Defensive Validation (Logs)
The WAF successfully triggered Rule 941110 (Category 1: Script Tag Vector). 
Evidence from `/var/log/apache2/error.log`:
`ModSecurity: Warning. Pattern match "(?i)<script[^>]*>" ... [severity "CRITICAL"]`

Tools Used
Server:Ubuntu (Apache2, MySQL, ModSecurity)
Attacker:** Kali Linux (Firefox, Burp Suite/Manual Injection)
