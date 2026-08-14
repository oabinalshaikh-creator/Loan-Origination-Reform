![Loan Origination Reform](assets/loan-origination-reform-full.jpg)

# Loan Origination Reform
### Product & Process Reform

> Rebuilding a legacy, sequential closing process into a parallelized, cloud-based, configurable system — cutting time-to-close from 15+ days to 5 without weakening compliance.

![Timeline](https://img.shields.io/badge/Time--to--Close-15%2B%20Days%20→%205%20Days-2D5F4C?style=flat-square) ![Domain](https://img.shields.io/badge/Domain-Loan%20Origination-1A2332?style=flat-square)

| ENGINEERING | PRODUCT | QA | DOMAIN |
|:---:|:---:|:---:|:---:|
| 20 | 4 | 4 | Loan Origination |

---

## The Problem

The origination process ran on legacy, on-premises technology that forced every application through the same rigid, fully manual path: intake, processing, document and income verification, underwriting, and closing, each stage waiting on the one before it regardless of how complete or straightforward the application already was.

Every application, however clean, was processed as if it needed the full manual treatment. There was no way to route a simple, complete file faster than a complex one, and no automation in the underwriting decision itself — every file waited on a human underwriter's manual review before it could move forward. The result was a closing timeline that regularly stretched past 15 days.

---

## Before & After

**Legacy Process — `15+ days`**

```
Manual Intake → Processing (Always Required) → Document & Income Verification → Underwriting (Manual Decision) → Closing
```
*Every application takes the full manual path, regardless of complexity.*

**Reformed Process — `5 days`**

```
AI-Enhanced Intake → Processing (If Needed) → Doc. & Income Validation → Qualification & Underwriting (Rules Engine) → Closing
```
*Intake → Processing (if needed) → Document & Income Validation → Qualification & Underwriting (Rules Engine) → Closing.*

---

## The Approach

The reform ran on several tracks at once, because fixing only the process without fixing the underlying decisioning and infrastructure would have capped how far the timeline could actually move.

**AI-Enhanced Intake**
Intake was enhanced, not automated. AI analyzes the borrower conversation and pre-fills the application from it, so the applicant isn't re-entering information they've already provided. A human still owns the intake step — the AI reduces the manual burden inside it rather than replacing it.

**Conditional Processing**
Processing was rebuilt as a conditional step rather than a default one. It now runs only when the AI-enhanced intake leaves gaps to fill, instead of treating every application as if it needs the same manual handling.

**Automated Income & Document Validation**
Income review, previously a fully manual step, was automated — extracting and validating income data directly from submitted documents rather than requiring a person to check it line by line.

**Rules-Engine Underwriting**
Built a rules engine that automates the underwriting decision at the qualification stage, applying the same lending and compliance criteria a human underwriter would, consistently and immediately, with manual review reserved for the applications the rules engine can't confidently clear.

**Cloud Migration & Configurability**
Moved the underlying systems off legacy on-premises infrastructure to the cloud, and rebuilt process and rules logic as configuration rather than hard-coded application logic — cutting the team's dependency on engineering for day-to-day process and rule changes.

**Compliance Review & Enhancement**
Compliance requirements were re-reviewed and built into the rules engine directly, with a full audit trail on every automated decision, so the faster process didn't come at the cost of audit coverage.

---

## Navigating the Friction

Two forms of resistance shaped how the rollout actually happened, and both had to be worked through rather than overridden:

<table>
<tr>
<td width="50%" valign="top">

**Compliance Sign-Off**
Handing the underwriting decision to a rules engine meant compliance needed confidence that the automated logic applied lending and regulatory criteria correctly and consistently — and that every decision left a clear, auditable trail. That confidence had to be earned through review and validation before sign-off, not assumed.

</td>
<td width="50%" valign="top">

**Team Control**
Underwriters and processors who had manually owned the qualification decision and the income review step were being asked to hand that judgment to automation. Getting buy-in meant involving them in defining the rules engine's logic and thresholds, so the system reflected their expertise rather than replacing it unilaterally.

</td>
</tr>
</table>

---

## Interface

> *Interface mockups below are illustrative reconstructions built to represent how the workflow functioned — not screenshots of the actual product, which remains confidential.*

<details>
<summary><b>Origination Pipeline Board</b> — <code>app.internal / origination / pipeline</code></summary>
<br>

| INTAKE (22) | PROCESSING (9) | DOC & INCOME (31) | QUALIFICATION (18) | CLOSING (12) |
|---|---|---|---|---|
| `LN-88231` · Day 1 · ✅ On Track | `LN-88198` · Gaps: 2 · 🟡 Needs Info | `LN-88175` · Day 2 · ✅ On Track | `LN-88190` · Rules Engine: Cleared · ✅ On Track | `LN-88110` · Day 4 · ✅ On Track |
| `LN-88240` · Day 1 · ✅ On Track | | `LN-88188` · Day 3 · 🟡 At Risk | `LN-88201` · Manual Review · 🟡 At Risk | `LN-88095` · Day 5 · ✅ On Track |

</details>

<details>
<summary><b>Ops Dashboard — Time to Close</b> — <code>app.internal / origination / ops-dashboard</code></summary>
<br>

| Avg Days to Close | Loans In Progress | SLA Compliance |
|:---:|:---:|:---:|
| **5.2d** | **142** | **96%** |

**Time-to-Close Trend**

| Baseline | Phase 1 | Phase 2 | Phase 3 | Phase 4 | Current |
|:---:|:---:|:---:|:---:|:---:|:---:|
| 15.4d | 13.1d | 10.6d | 8.2d | 6.4d | **5.2d** |

</details>

---

## Outcome

| 67% | 28 | 0 |
|:---:|:---:|:---:|
| **Faster Time-to-Close** | **Core Team, Delivered** | **Compliance Coverage Lost** |

Closing time dropped from 15+ days to 5 — a change that compounded across a high-volume loan pipeline. Beyond the headline number, the configurability work reduced ongoing dependency on engineering for process changes, and the compliance rework meant the faster process shipped with equal, not reduced, audit coverage.
