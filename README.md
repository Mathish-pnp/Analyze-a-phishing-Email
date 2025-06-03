# Task 2

# 🛡️ Task 2: Phishing Email Analysis Report

## 🎯 Objective
Analyze a suspicious email sample to identify common phishing characteristics and raise awareness of phishing tactics through technical investigation.

---

## 🧰 Tools Used

- 📧 Sample Phishing Email (open-source or educational purpose)
- 🔍 [MxToolbox Email Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)
- 🧠 Manual inspection for phishing indicators (language, links, sender address, etc.)

---

## 📬 Sample Email




---

## 🔍 Analysis and Phishing Indicators

| Indicator                     | Description |
|-------------------------------|-------------|
| **1. Spoofed Email Address** | The sender’s email domain (`secure-paypal.com`) closely mimics the legitimate `paypal.com`, indicating a spoofing attempt. |
| **2. Deceptive URL**         | Hyperlinked text says “Verify Now”, but hovering reveals a suspicious non-PayPal domain. |
| **3. Urgent Language**       | Threatens account suspension in 24 hours to create panic and force action. |
| **4. Generic Greeting**      | Uses “Dear Customer” instead of the recipient's actual name, a common phishing trait. |
| **5. Header Anomalies**      | Email header analysis showed failed SPF/DKIM authentication checks. |
| **6. Unsecured Link**        | Uses `http://` instead of `https://`, meaning the site isn’t encrypted. |
| **7. Social Engineering**    | Attempts to manipulate the user emotionally through fear and urgency. |

---

## 🛠️ Email Header Analysis Summary

Using MxToolbox Email Header Analyzer:
- **SPF:** Fail — The domain did not authorize the sending IP.
- **DKIM:** Fail — No valid DKIM signature found.
- **DMARC:** Fail — Misaligned domain policy.

These failures strongly indicate spoofing or misrepresentation.

---

## ✅ Conclusion

This email is a classic example of a phishing attempt using:
- A **spoofed sender address**,
- A **fake sense of urgency**,
- A **malicious verification link**, and
- **Authentication check failures** (SPF, DKIM, DMARC).

---

## 📢 Recommendations

- **Do NOT click** on suspicious links.
- **Verify** the sender's domain with official websites.
- **Report phishing** to the impersonated service (e.g., phishing@paypal.com).
- **Educate** employees and users on recognizing phishing attempts.
- **Use email filtering tools** to prevent phishing emails from reaching inboxes.

---

## 📁 Repository Structure


