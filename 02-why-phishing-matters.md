# Why Phishing Matters

## It is, by a wide margin, the #1 way attackers get in

Across nearly every major industry report on cybersecurity incidents, phishing and stolen or compromised credentials consistently rank as the leading initial access method used by attackers. Organizations spend enormous budgets hardening firewalls, patching servers, and deploying intrusion detection systems — and then an attacker bypasses all of it with a single convincing email that gets one employee to type a password into the wrong page.

This is why phishing deserves more attention in a security program than almost any other single topic: it is cheap for attackers to execute, difficult to fully prevent with technology alone, and devastating when it succeeds.

---

## A short history: why this attack has worked for almost 30 years

Phishing is not new, and understanding *why it has survived essentially unchanged for three decades* is one of the most important lessons in cybersecurity awareness.

### The 1990s: the birth of phishing

The technique traces back to the mid-1990s, when attackers on early online services like AOL began impersonating AOL staff in instant messages and emails, asking users to "verify" their account information or billing details. The term "phishing" itself appeared in hacker forums and newsletters around 1996. These early attacks were crude — bad grammar, obvious fake sender names — but they worked, because almost nobody was trained to question an email claiming to be from a trusted provider.

### The 2000s: phishing goes mainstream and targets money directly

As online banking and e-commerce exploded, phishing shifted from stealing AOL accounts to stealing banking credentials and credit card numbers. Fake bank login pages, fake PayPal "account suspended" emails, and fake eBay notices became a global criminal industry. This is also the decade when phishing kits — pre-built templates that let low-skill criminals clone a bank's login page in minutes — started circulating, turning phishing into a scalable business model rather than a one-off trick.

### The 2010s: phishing becomes targeted, corporate, and weaponized

This is the decade phishing stopped being just a consumer problem and became a **corporate espionage and fraud tool**. Attackers realized that one well-crafted email to the right employee could be worth more than thousands of generic blasts to random consumers. This gave rise to:

- **Spear phishing** — individually researched, personalized attacks against specific employees.
- **Business Email Compromise (BEC)** — impersonating executives to trick finance teams into wiring money.
- **Credential phishing as a precursor to ransomware** — instead of cashing out immediately, attackers used stolen logins to quietly explore a network, escalate privileges, and deploy ransomware weeks or months later.

High-profile breaches at major retailers, studios, and government agencies throughout this decade were traced back to a phishing email as the very first step in a much larger attack chain.

### The 2020s: AI, remote work, and industrialized phishing

Three forces converged in this decade to make phishing more dangerous than ever:

1. **Remote and hybrid work** dramatically increased the number of "plausible" IT and HR emails employees receive about VPNs, password resets, and account verification — exactly the pretexts phishing relies on.
2. **Generative AI** eliminated the old tell-tale signs of phishing (bad grammar, awkward phrasing, broken logos). Attackers can now generate flawless, personalized, native-language emails in seconds, and even clone a real executive's voice or video for vishing and deepfake-based fraud.
3. **Ransomware-as-a-Service (RaaS)** turned phishing into an industrialized supply chain: one group specializes in harvesting stolen credentials, another sells access to compromised networks, and a third deploys the actual ransomware — all connected through phishing as the common entry point.

### The pattern across 30 years

Notice what has **not** changed across this entire history: the attack still works by exploiting urgency, authority, and trust. What has changed is the attacker's *production quality* and *scale*. Phishing persists not because defenders haven't built good technology — they have — but because **the attack is aimed at a part of the system that technology can't fully patch: human judgment under pressure.**

---

## Where phishing stands today

Phishing has not slowed down — it has accelerated, and it increasingly targets large organizations, government bodies, and critical infrastructure rather than just individual consumers.

Key facts about the current threat landscape:

- Phishing volumes have risen sharply year over year, with industry anti-phishing tracking groups logging well over **one million phishing incidents in a single quarter** during 2025 — the highest level recorded since late 2023.
- The spread of infostealer malware delivered through phishing emails — malicious software designed specifically to harvest saved passwords, browser cookies, and session tokens — jumped dramatically in 2024, making stolen-credential attacks faster and easier to scale than ever.
- Large, well-known organizations across technology, finance, government, and retail have all suffered major phishing-driven incidents in the past two years, proving that **no sector and no company size is immune**: global technology companies, national tax authorities, financial institutions, and healthcare providers have all been hit.
- A significant share of companies surveyed globally report that employee credentials were compromised through a phishing attack within just the past year — making credential-phishing the single most commonly reported cause of security incidents in recent surveys.

The pattern is unmistakable: phishing is no longer a "spray and pray" nuisance. It is the preferred, most reliable entry point for some of the most damaging cyberattacks happening in the world right now, including ransomware outbreaks that take down hospitals, government agencies, and critical supply chains.

---

## A real, high-impact case: the Change Healthcare attack (2024)

To understand just how far-reaching a single phishing-style credential compromise can be, consider the **Change Healthcare cyberattack**, one of the most damaging healthcare cybersecurity incidents in U.S. history.

### What happened

In February 2024, a ransomware group known as **ALPHV/BlackCat** gained access to the network of Change Healthcare — a company that processes a massive share of medical claims and prescriptions across the entire United States healthcare system, and a subsidiary of UnitedHealth Group. The attackers got in using a **single set of stolen, compromised employee credentials**, obtained via credential-harvesting tied to a remote access portal that **did not have multi-factor authentication (MFA) enabled.**

Once inside, the attackers spent roughly nine days quietly moving through the network undetected, escalating privileges, and exfiltrating an estimated six terabytes of sensitive data — before finally deploying ransomware that encrypted critical systems and brought them down.

### The scale of the impact

- Change Healthcare ultimately confirmed that the personal and protected health information of approximately **190 million Americans** — close to six in ten people in the entire country — was exposed, including names, Social Security numbers, diagnoses, treatment details, and financial information.
- The attack caused **weeks of nationwide disruption** to pharmacies, hospitals, and medical billing systems, delaying prescriptions and payments for patients and providers across the country.
- UnitedHealth Group paid roughly **$22 million in ransom** to the attackers — and the attackers still did not fully protect the stolen data, which later resurfaced in extortion attempts by another criminal group.
- The total financial cost to UnitedHealth Group for response, recovery, and lost business reached well over **$3 billion**, making it one of the costliest cybersecurity incidents ever recorded for a single company.
- In Congressional testimony, UnitedHealth's own CEO confirmed publicly that the breach occurred because the compromised account lacked multi-factor authentication — a basic, inexpensive control that experts agree would very likely have stopped the attack outright.

### Why this case matters for every organization, big or small

This is not a story about a sophisticated, unstoppable nation-state hacking team breaking impenetrable systems. It is the story of **one compromised login, on one unprotected remote access point, that was never protected by a second layer of authentication.** From that single entry point, attackers caused a near-total shutdown of a critical piece of the U.S. healthcare system and over a billion dollars in direct losses.

The lesson for any company evaluating its own phishing risk is blunt: **the size of the consequence has nothing to do with the sophistication of the attack.** A credential obtained through a convincing but entirely ordinary-looking phishing email can be just as damaging as the most advanced piece of malware ever written — if the basic second layer of defense (MFA, verification, a trained employee who pauses and questions the request) isn't there to stop it.

---

## The bottom line

Phishing has survived for thirty years, across every technological era, because it targets something that does not get a software update: human trust under time pressure. It is cheap to launch, scales effortlessly, and — as the Change Healthcare case shows — a single successful attempt can cascade into consequences that affect millions of people and cost billions of dollars. That is why phishing awareness is not an optional "nice to have" training module. It is one of the highest-leverage investments an organization can make in its overall security posture.
