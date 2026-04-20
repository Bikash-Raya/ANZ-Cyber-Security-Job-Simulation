# Task 1: Email Analysis - Detailed Answers

## Email Analysis Framework

Before analyzing each email, I used the following framework:

- **S** - Sender verification
- **P** - Phishing indicators
- **A** - Attachments/Links analysis
- **M** - Message content review

---

## Email 1

### Classification: ✅ SAFE

### Screenshot
![Email 1](emails/email1.png)

### Analysis

| Indicator | Finding |
|-----------|---------|
| Sender | Adamm.johnnn1996@gmail.com - Personal Gmail account |
| Subject | Games Con trailers discussion |
| Links | None suspicious |
| Urgency | None |
| Request | No sensitive information requested |

### Detailed Justification

- **Context:** This is a casual conversation between two friends (Adam John and Velma Khan) discussing video game trailers from GamesCon, specifically KSP2 (Kerbal Space Program 2).

- **Sender Legitimacy:** The sender's email (Adamm.johnnn1996@gmail.com) is consistent with a personal account and matches the context of friendly communication.

- **Content Analysis:** The informal tone ("Hey mate", "Dude it looks sick as!!!", "You gonna buy the preorder?") is consistent with personal conversation between friends.

- **Red Flags:** None identified
  - No suspicious links
  - No attachments
  - No requests for sensitive information
  - No urgency tactics

### Verdict
This is a legitimate personal email between friends discussing shared interests. No action required.

---

## Email 2

### Classification: ❌ MALICIOUS

### Screenshot
![Email 2](emails/email2.png)

### Analysis

| Indicator | Finding |
|-----------|---------|
| Sender | Venture.ru - Russian domain |
| Subject | OneDrive Action Required |
| Links | "UPDATE YOUR ACCOUNT" button |
| Urgency | Yes - implies loss of functionality |
| Request | Account credentials |

### Detailed Justification

- **Sender Domain Red Flag:** The email is sent from "Venture.ru" - a Russian domain. Microsoft/OneDrive would NEVER send official communications from a .ru domain. Legitimate Microsoft emails come from:
  - @microsoft.com
  - @office365.com
  - @account.microsoft.com

- **Grammar and Professionalism:**
  - Poor grammar: "keep your office 365 E-mail address update"
  - Inconsistent capitalization
  - Generic, non-personalized content

- **Social Engineering Tactics:**
  - Creates urgency: "continue to receive large file"
  - Threatens loss of functionality
  - Uses legitimate-sounding branding (Office365 logo)

- **Malicious Intent:**
  - The "UPDATE YOUR ACCOUNT" button is designed to redirect to a credential harvesting page
  - Classic phishing attempt to steal Microsoft 365 credentials

### Attack Type
**Credential Phishing / Brand Impersonation**

### Recommended Action
- Do NOT click any links
- Report to IT Security team
- Delete the email
- Block sender domain

---

## Email 3

### Classification: ❌ MALICIOUS

### Screenshot
![Email 3](emails/email3.png)

### Analysis

| Indicator | Finding |
|-----------|---------|
| Sender | Vinny (no visible email) |
| Subject | Is Facebook working for you? |
| Links | facebook.com.opt/login.htm - FAKE |
| Urgency | Moderate - implies service issue |
| Request | Click link to "test" Facebook |

### Detailed Justification

- **URL Analysis - Critical Finding:**
