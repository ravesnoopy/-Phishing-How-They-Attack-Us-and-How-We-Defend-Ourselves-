# Simulated Phishing Examples Used in the Campaign

> ⚠️ **Important disclosure:** every email template below is entirely fictitious. No real company, bank, logo, or domain is reproduced here. These templates were built strictly for a controlled, authorized awareness simulation and are included in this repository purely for educational purposes. Running any simulated phishing campaign against real employees must always be formally authorized in writing by the organization's leadership, HR, legal, and IT/security teams beforehand, and should ideally be executed through a dedicated simulation platform (such as GoPhish, Microsoft Defender Attack Simulation Training, or a commercial awareness platform) rather than sent manually.

The three templates below were designed to represent three of the most common real-world phishing pretexts: a fake internal credential-theft page, a fake bank security alert, and a fake urgent password-change notice. Each one is broken down afterward to explain exactly which psychological levers (from `05-what-phishing-exploits.md`) it's built around.

---

## Example 1: Credential theft via a fake company login page

```
From: IT Support <support-it@corporate-notifications-portal.com>
To: employee@fictional-company.com
Subject: Action required: your mailbox has reached its storage limit

Hi [Name],

Your mailbox has reached 98% of its storage capacity. To avoid any 
interruption in receiving new emails, please verify your account using 
the secure link below before 6:00 PM today:

👉 Verify my account: hxxps://portal-fictionalcompany-login[.]com

If this step is not completed in time, your account may be temporarily 
suspended pending manual reactivation by the IT department.

Thank you,
IT Support Team
```

**What this clicks through to (in a real simulation):** a fake login page visually identical to the company's real single sign-on portal, capturing whatever username and password the employee enters, followed by an educational landing page explaining the exercise.

**Techniques used:**
- Urgency (a same-day deadline)
- Authority (impersonating the internal IT department)
- A domain that looks plausible at a glance but does not match the real company domain
- A consequence framed as inconvenience rather than danger, which lowers the recipient's guard ("my mailbox will stop working" feels low-stakes compared to "you've been hacked")

---

## Example 2: Fake bank security alert

```
From: Simulated Bank <alerts@simulatedbank-security.com>
To: customer@fictional-company.com
Subject: 🔒 We detected an unrecognized login attempt on your account

Dear Customer,

We detected a login attempt from an unrecognized device, located in a 
city you do not normally access your account from, at 3:42 AM.

If you do not recognize this activity, please verify your identity 
immediately to prevent unauthorized access:

👉 Confirm this was me: hxxps://simulatedbank-verification[.]net

If verification is not completed within 12 hours, your account will be 
temporarily locked for your protection.

Sincerely,
Security Department — Simulated Bank
```

**What this clicks through to (in a real simulation):** a fake banking portal requesting username, password, and — in a more advanced scenario — a one-time MFA code, demonstrating how even multi-factor authentication can potentially be defeated if a victim is tricked into relaying the code directly to the attacker in real time (a technique known as an MFA relay or "real-time phishing" attack).

**Techniques used:**
- Fear (unauthorized access is one of the most anxiety-inducing phrases in financial communication)
- Fabricated specificity (a fake location and timestamp make the threat feel concrete and real)
- A tight deadline that discourages the recipient from pausing to call the bank directly to verify

---

## Example 3: Urgent mandatory password change

```
From: System Administrator <admin@fictional-company-it.com>
To: employee@fictional-company.com
Subject: URGENT: You must update your password today

Hello,

Due to a security update to our internal systems, all employees are 
required to reset their password before 5:00 PM today.

Accounts that are not updated in time will be automatically locked, and 
reactivation will require submitting a request through HR, which may 
delay your system access by up to 48 hours.

👉 Update my password now: hxxps://fictionalcompany-resetpass[.]com

IT Systems Team
```

**What this clicks through to (in a real simulation):** a fake password-reset form that asks for the employee's *current* password (a major red flag that a real IT department would never need) along with a new one — demonstrating how attackers try to capture a working, currently valid credential rather than just any password.

**Techniques used:**
- Internal authority (impersonating the company's own IT department, which recipients are conditioned to comply with)
- A concrete operational penalty (losing system access, needing to go through HR) that feels more personally inconvenient than abstract
- A same-day deadline that discourages double-checking through a separate channel like a phone call or an in-person question to IT

---

## Red flags present across all three examples

| Red flag | Example 1 | Example 2 | Example 3 |
|---|---|---|---|
| Sender domain doesn't match the real organization | ✅ | ✅ | ✅ |
| Artificial urgency / tight deadline | ✅ | ✅ | ✅ |
| Direct request for credentials via a link | ✅ | ✅ | ✅ |
| Threat of a negative consequence (suspension, lockout) | ✅ | ✅ | ✅ |
| Generic or semi-personalized greeting | ✅ | — | ✅ |
| Appeal to fear / security concern | — | ✅ | — |
| Impersonation of an internal authority (IT) | ✅ | — | ✅ |
| Impersonation of an external authority (bank) | — | ✅ | — |

### How to train employees using these examples

When presenting these templates during an awareness session, the most effective approach is not simply to show the final email and say "this is fake." Instead, walk the audience through the red-flag table live, asking the room to identify each signal themselves before revealing it — active identification produces significantly better retention than passive viewing, which is one of the core findings in adult learning and security awareness research.
