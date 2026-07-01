# grc-risk-assessment
GRC Risk Assessment lab project using NIST CSF framework
# 🛡️ GRC Risk Assessment Lab

> **Cybersecurity Portfolio Project** — Governance, Risk & Compliance  
> Skill Level: Beginner | Time: 2–3 hrs | Cost: Free

---

## 📌 Project Overview

This project demonstrates a full **GRC Risk Assessment** for a fictional company (AcmeCorp), including:

- Asset inventory and classification
- Threat identification per asset
- Risk scoring using a **Likelihood × Impact** matrix
- Color-coded risk heatmap (Low / Medium / High / Extreme)
- Remediation recommendations mapped to **NIST CSF** controls

This mirrors what GRC analysts do daily at real organizations.

---

## 📁 Repository Structure

```
grc-risk-assessment/
├── README.md                  ← You are here
├── risk-register.csv          ← Full risk register (importable to Excel)
├── risk-matrix.md             ← Visual risk matrix + scoring guide
├── asset-inventory.md         ← Asset classification table
├── remediation-plan.md        ← Control recommendations per risk
└── report/
    └── grc-risk-report.md     ← Executive summary report
```

---

## 🎯 Scenario

**Organization:** AcmeCorp (fictional mid-size e-commerce company)  
**Scope:** IT infrastructure, customer data, internal systems  
**Framework:** NIST Cybersecurity Framework (CSF) + ISO 27001 aligned  
**Assessor:** [Your Name]  

---

## 🔢 Risk Scoring Methodology

```
Risk Score = Likelihood (1–5) × Impact (1–5)

Score Range   │ Rating   │ Color
──────────────┼──────────┼────────
1  – 4        │ Low      │ 🟢 Green
5  – 9        │ Medium   │ 🟡 Yellow
10 – 16       │ High     │ 🟠 Orange
17 – 25       │ Extreme  │ 🔴 Red
```

---

## 📊 Risk Matrix

|                 | **Impact 1** | **Impact 2** | **Impact 3** | **Impact 4** | **Impact 5** |
|-----------------|:---:|:---:|:---:|:---:|:---:|
| **Likelihood 5** | 🟡 5 | 🟠 10 | 🟠 15 | 🔴 20 | 🔴 25 |
| **Likelihood 4** | 🟢 4 | 🟡 8  | 🟠 12 | 🟠 16 | 🔴 20 |
| **Likelihood 3** | 🟢 3 | 🟡 6  | 🟡 9  | 🟠 12 | 🟠 15 |
| **Likelihood 2** | 🟢 2 | 🟢 4  | 🟡 6  | 🟡 8  | 🟠 10 |
| **Likelihood 1** | 🟢 1 | 🟢 2  | 🟢 3  | 🟢 4  | 🟡 5  |

---

## 🏆 Key Findings Summary

| Risk | Score | Rating |
|------|-------|--------|
| Unpatched public-facing web server | 20 | 🔴 Extreme |
| No MFA on admin accounts | 16 | 🟠 High |
| Customer PII stored unencrypted | 15 | 🟠 High |
| No offsite backup | 12 | 🟠 High |
| Weak password policy | 9 | 🟡 Medium |

---

## 🛠️ Tools Used

- Microsoft Excel / Google Sheets (risk register)
- NIST CSF Framework (nist.gov/cyberframework)
- MITRE ATT&CK (threat mapping)

---

## 📝 Resume Bullets

```
• Conducted GRC risk assessment for fictional e-commerce org using NIST CSF;
  identified 15 risks, prioritized by likelihood × impact scoring

• Built risk register mapping threats to assets with remediation controls
  aligned to ISO 27001 and NIST SP 800-53

• Produced executive risk report with color-coded heatmap and prioritized
  remediation roadmap
```

---

## 📚 References

- [NIST Cybersecurity Framework](https://www.nist.gov/cyberframework)
- [ISO/IEC 27001](https://www.iso.org/isoiec-27001-information-security.html)
- [MITRE ATT&CK](https://attack.mitre.org)
