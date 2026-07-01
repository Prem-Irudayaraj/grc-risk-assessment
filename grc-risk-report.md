# GRC Risk Assessment Report — AcmeCorp
**Prepared by:** [Your Name]  
**Date:** June 2026  
**Framework:** NIST Cybersecurity Framework (CSF)  
**Classification:** Internal Use Only

---

## Executive Summary

A comprehensive risk assessment was conducted for AcmeCorp's IT environment covering 8 critical assets. A total of **15 risks** were identified and scored using a 5×5 likelihood-impact matrix.

| Risk Rating | Count | % of Total |
|-------------|-------|------------|
| 🔴 Extreme  | 2     | 13%        |
| 🟠 High     | 8     | 53%        |
| 🟡 Medium   | 4     | 27%        |
| 🟢 Low      | 1     | 7%         |

**Overall Risk Posture: HIGH** — Immediate remediation required for 2 Extreme risks.

---

## Top 5 Priority Risks

### 1. 🔴 Unpatched Web Application Server (Score: 20)
- **Threat:** Remote code execution via CVE-2021-41773 (Apache 2.4.49)
- **Impact:** Full server compromise, data breach, service outage
- **Remediation:** Patch immediately; implement vulnerability scanning (Tenable/OpenVAS)
- **Timeline:** 24–48 hours

### 2. 🔴 SQL Injection on Customer Database (Score: 20)
- **Threat:** Attacker extracts full customer PII database
- **Impact:** Regulatory fines (GDPR/CCPA), reputational damage, customer loss
- **Remediation:** Parameterized queries, WAF tuning, penetration test
- **Timeline:** 1 week

### 3. 🟠 No MFA on Admin Accounts (Score: 16)
- **Threat:** Credential theft leads to full environment compromise
- **Impact:** Total loss of environment control
- **Remediation:** Enforce MFA via Azure AD / Okta
- **Timeline:** 1 week

### 4. 🟠 Hardcoded Credentials in Source Code (Score: 15)
- **Threat:** Developer commits DB password to GitHub — exposed publicly
- **Impact:** Database breach, lateral movement
- **Remediation:** Secret scanning (GitGuardian/GitHub Advanced Security), rotate all secrets
- **Timeline:** 1 week

### 5. 🟠 No MFA on Admin Accounts (Score: 16)
- **Threat:** Phishing email leads to account takeover
- **Impact:** Business Email Compromise, financial fraud
- **Remediation:** DMARC/DKIM/SPF, user awareness training
- **Timeline:** 2 weeks

---

## Remediation Roadmap

| Priority | Timeline | Actions |
|----------|----------|---------|
| **Immediate** | 0–48 hrs | Patch Apache server, review WAF rules |
| **Short-term** | 1–2 weeks | MFA rollout, secret rotation, email security |
| **Medium-term** | 1–3 months | EDR deployment, backup testing, pen test |
| **Long-term** | 3–6 months | Security awareness program, DLP, audit schedule |

---

## NIST CSF Gap Analysis

| Function | Maturity (1–5) | Key Gap |
|----------|---------------|---------|
| Identify  | 2 | No formal asset inventory process |
| Protect   | 2 | Missing MFA, encryption, patch mgmt |
| Detect    | 1 | No SIEM, no EDR |
| Respond   | 2 | Incident response plan not documented |
| Recover   | 2 | Backups not tested, no BCP |

---

## Conclusion

AcmeCorp faces significant cybersecurity risk, particularly around unpatched systems and lack of identity controls. Addressing the top 5 risks within 2 weeks would reduce the overall risk exposure by approximately **60%** and bring the organization to a defensible security posture.
