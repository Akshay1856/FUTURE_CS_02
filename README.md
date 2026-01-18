# 📧 Phishing Email Analysis – GitHub Impersonation Case Study

This repository documents a phishing email analysis based on two user-reported email screenshots that impersonate GitHub.  
The objective is to demonstrate **ethical email threat analysis**, phishing detection, and user awareness — **not hacking**.

## 🎯 Objective

The goal of this analysis is to:

- Analyze suspicious emails using **visual and header-based indicators**
- Identify common phishing techniques
- Classify email risk accurately
- Explain attacks in **simple, non-technical language**
- Provide **clear prevention and awareness guidelines** for users and employees

## 🧭 Scope & Ethics

✔ Publicly visible email content only  
✔ No links clicked  
✔ No attachments opened  
✔ No interaction with attacker infrastructure  

## 🛠️ Tools Used

### 1️⃣ Email Client Interface (Gmail UI)
Used to inspect:
- Displayed sender name
- Actual sender email domain
- Subject line and timestamps
- Email formatting and branding

### 2️⃣ Visual Header Indicators
While raw headers were not available, modern email clients expose **critical header indicators**, including:
- Sender domain mismatch
- Brand impersonation clues
- Email routing inconsistencies

### 3️⃣ Manual Domain Inspection
Used to:
- Compare the sender domain with legitimate brand domains
- Identify lookalike or unrelated domains
- Detect impersonation attempts

### 4️⃣ Browser Safety Techniques (Non-Intrusive)
- Hover inspection of buttons and links
- No clicking or redirection performed

## 🔍 Analysis Approach

1. **Sender Validation**
   - Compare the displayed sender name vs actual domain
   - Identify brand impersonation

2. **Header-Based Reasoning**
   - Assess likely SPF, DKIM, and DMARC failures
   - Detect misalignment with legitimate mail servers

3. **Content & Visual Analysis**
   - Review urgency cues
   - Analyse call-to-action behaviour
   - Inspect branding consistency

4. **Link & Action Review**
   - Identify hidden URLs behind buttons
   - Evaluate intent without clicking links

5. **Risk Classification**
   - Categorise email as Safe, Suspicious, or Phishing

## 📊 Key Findings Summary

| Indicator | Observation |
|--------|-------------|
| Brand impersonation | GitHub |
| Sender domain | `bigdogdomains.co` |
| Legitimate domain | `github.com` |
| Domain mismatch | ✔ |
| Hidden verification links | ✔ |
| Account urgency pressure | ✔ |

## 🚨 Email Risk Classification

**Final Verdict:** 🔴 **PHISHING**

**Reasoning:**
- Email impersonates GitHub
- GitHub does not own the sender domain
- Contains hidden verification links
- Attempts to harvest user credentials

## 🧠 How the Attack Works (Simple Explanation)

1. User receives an email that looks like GitHub  
2. Email requests urgent account verification  
3. User clicks the verification button  
4. User is redirected to a fake GitHub login page  
5. Credentials are stolen  

## 🛡️ Prevention & Awareness Guidelines

### ✅ Do’s for Users & Employees

✔ Always check the **sender’s domain**, not just the display name  
✔ Verify account alerts by visiting the website directly  
✔ Hover over links before clicking  
✔ Report suspicious emails to security teams  
✔ Enable multi-factor authentication (MFA)

### ❌ Don’ts for Users & Employees

❌ Do not trust logos or branding alone  
❌ Do not click verification links from unknown domains  
❌ Do not enter credentials from email links  
❌ Do not ignore sender mismatches  
❌ Do not forward suspicious emails

## 📢 Key Awareness Message
> **If an email claims to be from GitHub but is not sent from `@github.com`, it is a phishing attempt.**

## 📌 Conclusion

This case study highlights how phishing emails are used:
- Brand impersonation
- Domain spoofing
- Visual deception
- Urgency and fear

Basic inspection of sender domains and cautious user behaviour can prevent most phishing attacks.

---

## ⚖️ Disclaimer

This repository is for **educational and awareness purposes only**.  
No real phishing infrastructure was accessed or interacted with.

⭐ If this repository helped you understand phishing detection, feel free to star it.
