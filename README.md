# External Attack Surface Mapping & OSINT Assessment

## 📌 Project Overview
This repository contains a comprehensive Passive Reconnaissance and Open-Source Intelligence (OSINT) report conducted as an academic project at the Military University of Technology (WAT). The objective was to map the external attack surface of a live e-commerce target and identify potential security misconfigurations.

> **⚠️ DISCLAIMER:** This audit was performed using **strictly passive, publicly available tools (OSINT)** for educational purposes. No active scanning, exploitation, or intrusive testing was conducted against the target's infrastructure.

## 🛠️ Tools & Technologies Used
* **Infrastructure Analysis:** DNSDumpster, Shodan, Censys, Netcraft, IPinfo
* **Web Application Analysis:** Wappalyzer, BuiltWith, SecurityHeaders, Qualys SSL Labs
* **Data Breaches & Threat Intel:** HaveIBeenPwned, VirusTotal, AbuseIPDB, Leak-Lookup
* **Metadata & OSINT:** Google Dorks, ExifTool / Metadata2go, HR OSINT

## 🔎 Key Findings Overview
By analyzing publicly accessible data, the following vulnerabilities and misconfigurations were identified:
* **DNS Misconfigurations:** Absence of DMARC and SPF policies, exposing the domain to email spoofing and phishing campaigns.
* **Exposed Environments:** Discovery of a publicly accessible development sub-domain sharing the same IP address as the production environment.
* **Credential Leaks:** Located compromised corporate email credentials in public data breaches (e.g., the Nitro PDF breach).
* **Architecture Flaws:** Detected missing security headers (HSTS, CSP, X-Frame-Options) exposing users to client-side attacks.

## 🛡️ Proposed Mitigation Strategies
The report concludes with actionable recommendations, including:
1. Implementation of robust DMARC and SPF records.
2. Mandatory password rotation and Multi-Factor Authentication (MFA) enforcement for all corporate accounts.
3. Web server hardening and restriction of public access to development environments.

---
**📄 The full detailed report (in Polish) can be found in the attached PDF file.**
