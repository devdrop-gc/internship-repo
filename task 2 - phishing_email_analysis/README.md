# 🔍 Phishing Email Analysis

## 🎯 Objective
Identify phishing characteristics in a suspicious email sample.

## 🧰 Tools Used
- MX Toolbox – Header Analyzer
- IP / Geolocation Lookups

---

## 📘 What I Did
### 1. Used a Real Phishing Email
- Pulled from a verified educational source (Nebraska GenCyber Phishing Module).
- Included original, unmodified headers for authenticity.
### 2. Analyzed Technical Indicators
- Checked for sender spoofing and mismatched domains.
- Traced the header path to identify relay anomalies.
- Reviewed originating IP address and its geolocation.
### 3. Inspected Social Engineering Tactics
- Noted grammar and spelling errors.
- Identified urgency-based language.
- Flagged psychological manipulation (fear, authority, reward).
### 4. Ran Headers Through MX Toolbox
- Documented all lookup results.
- Captured screenshots from the analyzer tool.
- Highlighted SPF/DKIM/DMARC failures and suspicious routing.

---

## 📈 Summary

| Indicator | Evidence |
|---------|----------|
| Spoofing | Mismatched domains |
| No Auth | SPF fail |
| Proxy | Israel → Taiwan |
| Greed | $18M offer |
| Grammar | Multiple errors |

---

## 📦 Repository Contents
- `sample_email.txt` – Raw phishing email  
- `email_headers.txt` – Headers extracted for analysis  
- `analysis_report.md` – Step-by-step phishing indicators  
- `screenshots/` – Header analyzer Tool output 


**Sample Source:** Nebraska GenCyber Phishing Module (educational use only).
