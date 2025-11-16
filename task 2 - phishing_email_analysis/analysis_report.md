# Phishing Email Analysis Report

**Sample:** Advance-fee scam (419)  
**Source:** Nebraska GenCyber (educational)

---

## 1. Obtain Sample
- Full email: `sample_email.txt`  
- Email Headers: `email_headers.txt`

---

## 2. Sender Spoofing

| Field | Value | Red Flag |
|------|-------|----------|
| `From` | `vieria@aol.com` | Free provider |
| `Reply-To` | `carrr444@yahoo.com` | Mismatch |
| `Return-Path` | `32309uslisidfj@mail.shako.com.tw.com` | Gibberish |

---

## 3. Header Analysis (MX Toolbox)

**Input file:** `email_headers.txt`  
**Results:**  
- **SPF:** Neutral (fail)  
- **SpamScore:** 73  
- **X-FOSE-spam:** "This message appears to be spam."

**IP Geolocation:**

| IP | Location | Country | ISP |
|----|--------|--------|-----|
| `85.250.54.29` | Kiryat Ono | Israel | Cellcom |
| `59.125.100.112` | Taipei | Taiwan | Chunghwa |
| `59.125.100.113` | Taipei | Taiwan | Chunghwa |
| `65.55.88.116` | Hong Kong | Hong Kong | Microsoft |

**Red Flag:** Path **Israel → Taiwan → US** – not in Africa.

---

## 4. Links / Attachments
- None  
- Contact: `00233 244 617 863`, `carrr444@yahoo.com`

---

## 5. Urgency / Threats
- Greed: **30% of $60M**  
- Tragedy: "father short dead by rebels"

---

## 6. Mismatched URLs
- N/A

---

## 7. Grammar Errors
- "short dead" → "shot dead"  
- lowercase "i"  
- run-on sentences

---

## 8. Summary

| Indicator | Evidence |
|---------|----------|
| Spoofing | Mismatched domains |
| No Auth | SPF fail |
| Proxy | Israel → Taiwan |
| Greed | $18M offer |
| Grammar | Multiple errors |

**Conclusion:** Confirmed **phishing scam**.