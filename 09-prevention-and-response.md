# How to Prevent Phishing, and What to Do When It Happens Anyway

No organization can reduce phishing risk to zero — the Change Healthcare case in `02-why-phishing-matters.md` is a stark reminder that a single compromised credential can cause billions of dollars in damage even at a massive, resource-rich company. The goal of a mature security program is not an unrealistic "we'll never get phished" promise. It's building **layered defenses that catch an attack at multiple points**, and a clear, judgment-free response process for the moment something does slip through.

---

## Part 1: Prevention — organizational controls

### Technical controls

- **Multi-factor authentication (MFA) everywhere it matters** — email, VPN, and any system handling sensitive data or payments. This is, by a wide margin, the single highest-leverage control available. In the Change Healthcare breach, the compromised account that led to a $3+ billion incident did not have MFA enabled on its remote access point. A second authentication factor would very likely have stopped the entire chain of events before it started.
- **Domain authentication — SPF, DKIM, and DMARC** configured on the company's email domain, ideally with a DMARC policy set to `quarantine` or `reject` rather than just monitoring, so spoofed emails impersonating the company's own domain are actually blocked rather than just logged.
- **Advanced email filtering** with attachment sandboxing and real-time link analysis, which can catch a meaningful share of phishing attempts before they ever reach an inbox.
- **A corporate password manager** to eliminate password reuse across accounts — a major factor in how a single leaked credential from one breach ends up enabling access to unrelated systems elsewhere.
- **Least-privilege access** — ensuring employees and especially service/remote-access accounts only have the minimum system access required for their role, so that a single compromised account has a smaller blast radius if it is breached.
- **Endpoint detection and response (EDR)** tools that can catch unusual behavior (like an infostealer harvesting saved passwords) even after an attachment has already been opened.

### Process and policy controls

- **Out-of-band verification for payments** — any request to pay an invoice, change a vendor's bank details, or process an urgent wire transfer must be confirmed through a second, independent channel (a phone call to a known number, an in-person check) before it's executed, no matter how urgent or how senior the requester appears to be.
- **A clear, no-blame reporting process** — a one-click "Report Phishing" button in the email client, or a dedicated, well-publicized reporting inbox, with an explicit policy that reporting is never penalized, even if the employee already clicked or entered data.
- **Regular, recurring simulated phishing campaigns** — not a one-time event, but an ongoing program, so the organization has continuously updated, real data on where its risk actually lives (see `08-campaign-results-and-department-risk.md` for how to structure and interpret that data).
- **Department-specific training**, built around the actual attack patterns each role faces — generic company-wide training alone consistently underperforms targeted training built around real departmental risk.
- **An incident response plan that's actually been rehearsed**, not just written and filed away — including clear ownership of who does what in the first hour after a suspected compromise is reported.

---

## Part 2: What every employee should do

### If you receive a suspicious message

1. **Don't click.** Not even "just to see" — simply opening a link can sometimes be enough to trigger tracking or, in rarer cases, exploit a browser vulnerability.
2. **Don't reply, and don't forward it to anyone except security/IT.** Replying confirms to the attacker that your address is active and monitored, which can lead to more targeted follow-up attempts.
3. **Verify independently if the sender seems legitimate.** Call the person or department using a phone number you already know — never one provided in the suspicious message itself.
4. **Report it** through the official channel, every time, even if you're not fully sure it's malicious. A false positive costs the security team a few minutes of review. A missed real attack can cost the entire company far more.
5. **Give a heads-up to your team** if the pretext seems like something that could plausibly be sent to your colleagues too — a shared early warning can stop a wider campaign in its tracks.

### If you already clicked, entered data, or opened an attachment

1. **Change your password immediately**, from a different, trusted device if possible.
2. **Report it to security/IT right away, without hesitation.** Speed matters enormously here — the faster a real compromise is reported, the faster it can be contained before an attacker escalates from a single stolen credential to a much larger breach (exactly the pattern described in `04-how-phishing-attacks.md`).
3. **If you entered financial information**, contact your bank or card issuer immediately to flag potential fraud.
4. **Check if you reused that same password anywhere else**, and change it there too — credential reuse is one of the most common ways a single phishing success turns into multiple compromised accounts.

### The golden rule

**Stop. Think. Verify. Report.**

This single four-step habit, repeated consistently across an entire organization, is worth more than almost any individual piece of security software. Technology can filter out a large share of phishing attempts before they ever arrive — but for the ones that get through, the employee who pauses for ten extra seconds before clicking is the last and most important line of defense.

---

## Why a judgment-free culture is a prevention control, not just a nice-to-have

It's tempting to treat phishing training as purely technical: teach people the red flags, test them, move on. But the data consistently shows that **how an organization reacts to mistakes shapes whether future mistakes get reported at all.** A culture that publicly shames or penalizes employees who fall for a simulated (or real) phishing attempt teaches people to hide their mistakes — which means the next *real* attack goes unreported, undetected, and uncontained for far longer than it should. A culture that treats reporting as valuable, even for an employee's own mistake, dramatically shortens the time between a real compromise and the moment security becomes aware of it — which, as the Change Healthcare case shows, can be the single biggest factor separating a contained incident from a billion-dollar catastrophe.
