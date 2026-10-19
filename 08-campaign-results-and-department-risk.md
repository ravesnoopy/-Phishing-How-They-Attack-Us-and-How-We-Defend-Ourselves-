# Campaign Results and Department-by-Department Risk Analysis

> 📊 **Note on the data below:** the numbers in this section are simulated/fictitious, created to illustrate the format and structure a real reporting deliverable should follow. Replace them with your own campaign's real, anonymized results before presenting them internally.

---

## Metrics that actually matter in a phishing campaign

Before looking at the results table, it's worth being explicit about *why* each metric is tracked, because the metrics tell very different stories depending on how they're combined.

| Metric | Formula | What it tells you |
|---|---|---|
| Open rate | opened ÷ sent | How effective the subject line / sender was at getting attention |
| Click rate | clicked ÷ sent | Baseline susceptibility to the lure |
| Data-entry rate | entered credentials ÷ sent | The most critical risk metric — this is where real damage happens |
| **Report rate** | reported ÷ sent | **The single most important metric** — it measures security culture, not just vulnerability |
| Time to first report | minutes from send to first report | How fast the organization could realistically detect a real attack |
| Repeat-click rate | employees who click across multiple campaigns | Who specifically needs reinforced, individual coaching |

The report rate deserves special emphasis: an employee who clicks a simulated phishing link but immediately reports it to security has actually demonstrated *good* instincts under a difficult, well-designed test — and in a real attack, their report could trigger a fast organizational response that limits the damage. A department with a high click rate but also a high report rate is, counterintuitively, often in better shape than a department with a low click rate and almost no reporting at all, because the second group has no habit of flagging suspicious activity when it matters.

---

## Simulated results by department

| Department | Emails sent | Click rate | Credentials entered | Reported to security | Risk level |
|---|---|---|---|---|---|
| Finance | 40 | 35% | 18% | 10% | 🔴 High |
| Human Resources | 35 | 42% | 22% | 8% | 🔴 High |
| IT | 20 | 10% | 2% | 55% | 🟢 Low |
| Operations | 50 | 28% | 12% | 20% | 🟡 Medium |
| Sales | 30 | 30% | 15% | 15% | 🟡 Medium |
| Executive Leadership | 8 | 25% | 12% | 12% | 🟡 Medium (high blast radius) |

### Quick reading of the results

- Finance and HR together account for the **highest combined risk** (click rate + credential entry), and both also show the **lowest reporting rates**, which compounds the danger — not only are these departments more likely to fall for an attack, they're also the least likely to flag it quickly if it's real.
- IT has by far the lowest click rate, but more importantly, the **highest report rate by a wide margin** — this is a strong signal that technical familiarity alone doesn't explain the gap; deliberate reporting habits do.
- Executive Leadership has a small sample size, but a single successful attack against this group carries disproportionate impact (see whaling, in `03-types-of-phishing.md`), so its risk should never be evaluated purely by percentage — it needs to be weighted by potential damage.

---

## Why attacking HR is a fundamentally different threat than attacking Finance

This is one of the most important insights for designing department-specific training, and it's frequently missing from generic, one-size-fits-all awareness programs: **phishing is not generic. Attackers design the pretext around what a specific role has access to, and the consequence of a successful attack is completely different depending on the target.**

| | **Human Resources** | **Finance** |
|---|---|---|
| **What they have access to** | Personal employee data, payroll records, contracts, résumés and attachments from unknown external senders | Bank accounts, vendor payments, wire transfer approval, banking detail changes |
| **Typical attacker pretext** | "Please find my résumé attached," fake termination/leave requests, payroll complaints | Fake invoices, vendor bank-account change requests, urgent CEO-requested wire transfers (BEC) |
| **Impact if compromised** | Personal data exposure (regulatory/compliance exposure), malware delivered via malicious attachments | **Direct, immediate financial loss** — wired money is extremely difficult to recover |
| **Why they're easier to trick** | Receiving unsolicited attachments from strangers (résumés) is a normal, expected part of the job | Routine time pressure around payment cycles and recurring approval processes |
| **Dominant attack type** | Malware via document attachment / personal-data-focused phishing | Business Email Compromise (BEC) / fake invoice fraud |
| **Typical consequence** | Regulatory fines, reputational damage, employee trust erosion | Immediate, often unrecoverable monetary loss |

### The core takeaway

Because HR and Finance face structurally different attacks with structurally different consequences, **a single generic "here's what phishing looks like" presentation to the whole company is not enough.** HR needs specific training on attachment hygiene and personal-data-handling procedures. Finance needs specific training on payment-verification protocols and how BEC attacks look different from traditional credential-phishing (often no link, no attachment — just a convincing, well-timed request). Treating every department identically wastes the most valuable targeting insight a campaign produces: **who is being attacked, how, and why.**

### How to use this for prioritization

When deciding where to invest limited training time and budget, combine two factors from the results table: **susceptibility** (click + credential-entry rate) and **blast radius** (what that department's access could cost the company if compromised). A department that is both highly susceptible *and* high-access — as Finance and HR both are in this simulated data — should always be the first priority for targeted, role-specific training, well ahead of departments that are merely susceptible but have limited access to sensitive systems or funds.
