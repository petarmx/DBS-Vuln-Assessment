# 🔓 Database Server Vulnerability Assessment  
*E-Commerce Company | 28th June 2025*

---

## 🏢 [Scenario Overview](https://github.com/petarmx/DBS-Vuln-Assessment/blob/32d7859a32fd1e09a7bbe7c214bc101787e51577/Scenario.pdf)

**Role:** Newly Hired Cybersecurity Analyst  
**Company:** E-Commerce Enterprise (Global Remote Workforce)  
**Key Issue:** Database server has been publicly accessible since launch, exposing sensitive customer and business data.

---

## 🐧 System Description

- **Hardware:** Powerful CPU, 128GB RAM  
- **OS:** Latest Linux  
- **Database:** MySQL  
- **Network:** IPv4, SSL/TLS encrypted connections  
- **Interaction:** Connects with other business servers

---

## 🔍 Scope

- **Focus:** Access controls and security posture of the database server  
- **Assessment Period:** June 2025 – August 2025  

---

## 🎯 Purpose

- **Business Value:** Central repository for customer and sales data, essential for remote sales and marketing operations.  
- **Security Importance:** Protects sensitive data from theft, regulatory penalties, and reputational damage.  
- **Impact of Disruption:** Server downtime would halt global sales, customer support, and analytics, causing significant financial and operational harm.

---

## ⚠️ Risk Assessment [(Full Report)]([https://github.com/petarmx/DBS-Vuln-Assessment/blob/32d7859a32fd1e09a7bbe7c214bc101787e51577/Vulnerability%20assessment%20report.pdf)

| Threat Source         | Threat Event                        | Likelihood | Severity | Risk |
|----------------------|--------------------------------------|------------|----------|------|
| External Attacker    | Data exfiltration via public DB      | 3          | 3        | 9    |
| Malicious Insider    | Unauthorized data manipulation       | 2          | 3        | 6    |
| Accidental Exposure  | Sensitive data leakage               | 2          | 2        | 4    |

---

## 🛠️ Approach

- **Risk Selection:** Prioritized threats exploiting public server access.  
- **Scoring Basis:**  
  - **Likelihood:** Exploit feasibility (public DB = High; internal = Medium)  
  - **Severity:** Financial/operational impact (FAIR model)  
- **Limitations:** Excluded physical security and third-party integrations.

---

## 🛡️ Remediation Strategy

### Immediate Actions

1. **Close public access** via IP whitelisting (corporate VPNs only).
2. **Enforce multi-factor authentication (MFA)** for all database users.

### Technical Controls

- **Role-based access controls** (minimum privilege principle).
- **Encrypt data in transit** with TLS (upgrade from SSL).
- **IP allow-listing** to corporate offices.

### Operational Improvements

- **Monthly vulnerability scans.**
- **Employee training** on phishing/social engineering risks.
- **Regular backup verification.**

### Managerial Controls

- **Establish SLA policies** for critical patching
- **Quarterly audits** tracking open/closed vulnerabilities.

---

## 📝 Executive Summary

**The publicly accessible database server presents critical risks, including data exfiltration and operational disruption. Immediate access restriction and MFA implementation are prioritized to reduce breach risk. Continuous monitoring and employee training will sustain security improvements.**

---

## 🛡️ NIST CSF Alignment

| Function  | Actions & Improvements                                      |
|-----------|------------------------------------------------------------|
| Identify  | Regular audits, asset inventory, risk identification       |
| Protect   | Firewall rules, MFA, role-based access, encryption         |
| Detect    | Monitoring, vulnerability scans, anomaly detection         |
| Respond   | Incident response procedures, communication protocols      |
| Recover   | Backup/recovery testing, post-incident review              |

---

## 📂 Conclusion

By addressing the public access vulnerability and implementing robust authentication, access controls, and monitoring, the company can significantly reduce its risk of data breaches and operational disruption. Ongoing security assessments and staff training are essential for maintaining a strong security posture.

