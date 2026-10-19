# Types of Phishing

Phishing is not a single technique — it's a family of attacks that share the same psychological core (impersonation + urgency + a specific ask) but adapt to whatever channel, context, or target gives the attacker the best odds of success. Understanding the different forms matters because **each one requires a slightly different defense.**

---

## 1. Email phishing (the classic)

The original and still the most common form: a generic, mass-distributed email impersonating a well-known brand, service, or internal department, sent to as many addresses as possible. It relies on volume — if only 1-2% of recipients fall for it, a campaign of 100,000 emails still nets a meaningful number of victims.

**Typical pretexts:** account suspension notices, fake invoices, shipping notifications, "your mailbox is full" alerts.

---

## 2. Spear phishing

A targeted, researched attack aimed at a specific individual or small group, using real details gathered from LinkedIn, company websites, social media, or previous data leaks to make the message far more convincing than a generic blast. A spear phishing email might reference your actual manager's name, a real project you're working on, or a recent company announcement.

**Why it's more dangerous:** the personalization dramatically increases the click-through rate, because the usual red flags (generic greeting, irrelevant content) are gone.

---

## 3. Whaling

A specialized form of spear phishing aimed specifically at senior executives, directors, or other high-value, high-authority targets ("the big fish"). Because executives often have broader system access, approval authority over large payments, and less day-to-day oversight of their own inbox, a successful whaling attack tends to produce outsized damage.

**Typical pretext:** a fake legal subpoena, a board-level "confidential" request, or an urgent personal matter requiring immediate action.

---

## 4. Business Email Compromise (BEC)

One of the most financially damaging phishing categories. The attacker impersonates — or actually gains control of — an executive's or vendor's real email account, then instructs an employee (usually in finance or accounts payable) to urgently wire money or change banking details for an upcoming payment.

**What makes BEC different:** it often contains no malicious link or attachment at all, which means traditional email security filters (built to catch malware and bad URLs) frequently let it through untouched. The entire attack is pure social engineering, delivered in plain text.

---

## 5. Smishing (SMS phishing)

Phishing delivered via text message, typically impersonating a delivery company, a bank's fraud alert system, or a government agency. Smishing exploits the fact that people tend to trust text messages more than email and often read them on a small screen where a fake link is harder to scrutinize.

**Typical pretext:** "Your package could not be delivered, confirm your address," or "Unusual activity detected on your card."

---

## 6. Vishing (voice phishing)

Phishing carried out over a phone call, often impersonating a bank's fraud department, tech support, or — increasingly — a company's own IT help desk. Modern vishing attacks sometimes use AI-based voice cloning to impersonate a real executive's voice convincingly enough to authorize a fraudulent transaction over the phone.

**Why it's growing fast:** voice carries a sense of real-time urgency and authenticity that's harder to fake-check in the moment, especially under pressure.

---

## 7. Quishing (QR code phishing)

A newer technique where a malicious QR code — placed on a poster, a parking meter, a fake delivery notice, or even sent by email as an image — redirects a scanning smartphone to a fraudulent website. Quishing is particularly effective because QR codes hide the destination URL from the user until after they've already scanned it, and many corporate email security filters are not yet tuned to scan the *content* of an image for a malicious link.

---

## 8. Pharming

A more technical variant where the attacker compromises DNS settings or a router/device configuration so that even when a victim types the *correct* website address, they're silently redirected to a fake copy of that site. Unlike most phishing, pharming requires no click on a suspicious link — the victim can do everything "right" and still land on a fraudulent page.

---

## 9. Clone phishing

The attacker intercepts or copies a real, previously delivered legitimate email — keeping the original formatting, sender name, and content nearly identical — but swaps out a link or attachment for a malicious one, then resends it as if it were an update or a resend of the original message. Because it looks like something the recipient has already seen and trusted once, clone phishing has a notably higher success rate.

---

## 10. Angler phishing (social media phishing)

Attackers monitor social media for people publicly complaining to a company (an airline, a bank, an e-commerce platform) and respond pretending to be that company's official support account, redirecting the frustrated customer to a fake "support" page to "resolve" their issue — capturing credentials or payment details in the process.

---

## Quick comparison table

| Type | Primary channel | Target scope | Key danger |
|---|---|---|---|
| Email phishing | Email | Mass / broad | High volume, low cost for attacker |
| Spear phishing | Email | Individual | Highly convincing, personalized |
| Whaling | Email | Executives | High-value, high-authority targets |
| BEC | Email | Finance / AP teams | Often bypasses malware filters entirely |
| Smishing | SMS | Mass / broad | Exploits trust in text messages |
| Vishing | Phone call | Individual / broad | Real-time pressure, voice cloning risk |
| Quishing | QR code | Mass / broad | Hides destination until too late |
| Pharming | DNS / network | Mass | Works even with a correctly typed URL |
| Clone phishing | Email | Individual / broad | Reuses an already-trusted message |
| Angler phishing | Social media | Individual | Exploits public frustration and urgency |

---

## Why this matters for a defense strategy

A security awareness program that only trains employees to spot a *suspicious email* is incomplete. Modern attackers deliberately pick whichever channel is least defended inside a given organization — if email filtering is excellent but nobody has ever discussed vishing, that's exactly the gap a motivated attacker will exploit. Effective training has to cover the full channel landscape, not just the inbox.
