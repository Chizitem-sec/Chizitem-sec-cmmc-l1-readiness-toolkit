# CMMC Level 1 Readiness Toolkit

A practitioner's reference library for the **15 requirements of CMMC Level 1** (58 assessment objectives) — the cybersecurity baseline that protects **Federal Contract Information (FCI)** for organizations in the U.S. Defense Industrial Base. For each requirement, the toolkit answers the questions a small business (and its assessor) actually asks: *who owns it, what it means, how it's audited, what evidence proves it, what to ask, and when it doesn't apply* — plus how each requirement maps to the commercial frameworks (**SOC 2** and **ISO 27001:2022**) those same businesses often need next.

> **Author:** Johnbosco Ibeneme · **Focus:** Governance, Risk & Compliance (GRC) · CMMC / NIST 800-171 / SOC 2 / ISO 27001

---

## Start here

| If you want to… | Open |
|---|---|
| See all 15 requirements at a glance, with commercial mappings | **`CMMC_L1_Master_Readiness_Library.xlsx`** |
| See how one requirement gets worked end to end | **`deep-dives/CMMC_L1_DeepDive_SC_and_AC.pdf`** |
| Understand the reasoning behind the commercial mappings | [Primary vs. Supporting](#primary-vs-supporting-how-the-commercial-mappings-are-built), below |
| Understand when "Not Applicable" is legitimate | [A note on "Not Applicable"](#a-note-on-not-applicable), below |

The workbook is the **library**; the deep-dives are what a single row looks like when you **work it**. The workbook tells you what the control is and where it maps. The deep-dive shows the reasoning, the evidence, and the judgment calls that a spreadsheet cell can't hold.

---

## Why this exists

Most CMMC tooling tells you *whether* a requirement is met. It rarely tells a non-expert *how to know*. This toolkit closes that gap with a single, repeatable structure applied consistently across all 15 Level 1 requirements, so a small business can self-assess honestly and an assessor can follow the reasoning.

It also does something most CMMC references don't: it **maps every requirement to its SOC 2 and ISO 27001 equivalents.** Federal and commercial compliance are the same discipline in different dialects — a large share of the substance overlaps. Showing that overlap turns "we did CMMC" into "we have a control baseline that ports to the commercial audits our customers ask for."

One caveat stated up front, because it matters more than the overlap: **conceptual overlap is not audit equivalence.** CMMC Level 1 asks whether a control *exists*. SOC 2 asks whether it was designed appropriately and *operated effectively over a review period*. ISO asks whether it lives inside a functioning management system. A control can map cleanly across all three and still leave an organization nowhere near certified in two of them. The mappings here are a running start, not a shortcut.

---

## What's in this repo

**`CMMC_L1_Master_Readiness_Library.xlsx`** — all 15 requirements in one workbook, 16 columns, every section of the template as a column. The master reference. Includes the full NIST SP 800-171A assessment objectives for each requirement (58 total), N/A eligibility, and four separate commercial-mapping columns: SOC 2 Primary, SOC 2 Supporting, ISO 27001 Primary, ISO 27001 Supporting.

**`deep-dives/`** — full-page worked sheets for the two requirements with real N/A nuance:

- **Public-Access System Separation (SC.L1-b.1.xi · NIST 3.13.5)** — the one Level 1 requirement where N/A is frequently legitimate. Worked with the full determination / boundary-logic / re-evaluation-trigger structure.
- **Control Public Information (AC.L1-b.1.iv · NIST 3.1.22)** — a *conditional* N/A case, which is the harder and more common judgment call.

Together they show the spectrum: one requirement where N/A is often right, one where it usually isn't but occasionally is.

**`README.md`** — this file.

---

## The structure (every requirement follows the same 8 sections)

| # | Section | What it answers |
|---|---------|-----------------|
| 0 | **Identity** | Practice statement, level, source citation, and the formal assessment objectives ([a], [b], …) |
| 1 | **Intent** | What the requirement is really asking for, in plain language |
| 2 | **Ownership** | Who is *Responsible* (does it) vs *Accountable* (owns the outcome) |
| 3 | **Assessment** | How an assessor audits it — Examine / Interview / Test |
| 4 | **Evidence** | The artifacts to have ready (final, approved — drafts are not valid evidence) |
| 5 | **Customer Questions** | Tiered questions to determine status (scope → implementation → evidence) |
| 6 | **Not Applicable** | Honest N/A eligibility, the three-part determination, and defensible verbiage |
| 7 | **Commercial Mapping** | SOC 2 (TSC) and ISO 27001:2022 Annex A equivalents, split Primary / Supporting |

---

## Primary vs. Supporting — how the commercial mappings are built

Every mapping in this toolkit names a **Primary** and, where one exists, a **Supporting** criterion. That split is deliberate, and it's the part of this toolkit that took the most thought.

- **Primary** = where the control's protective purpose sits — the criterion that most directly describes what the control does.
- **Supporting** = criteria the control contributes evidence toward, and that an auditor will also want to see.

The reason for the split: a crosswalk has two jobs and they don't have the same answer. *Which criterion describes the mechanism?* is usually a narrow, specific one. *Which criterion will an auditor actually test you against?* is often a broad one. Mapping everything to the broadest criterion is technically correct and practically useless — it tells a team nothing about what evidence to pull. But mapping only to the tightest mechanism under-prepares evidence for the criterion an assessor examines most directly. Naming both, and saying which job each is doing, is what makes the crosswalk usable by someone who didn't build it.

This also means the broad criterion isn't banned. For **SC.L1-b.1.xi** (public-access system separation), SOC 2 **CC6.1** is the *Primary* — because its points of focus expressly address network segmentation. The same criterion is deliberately *not* primary elsewhere. Mapping is case-by-case evidence-seeking, not rule-following.

A related test used throughout: **if a vendor changed their product architecture tomorrow, would the mapping still hold?** If it only works because of how a specific product happens to be built, it's a technology overlap, not a control mapping.

Where a Supporting cell has no criterion, the cell says so and explains why rather than sitting blank — a deliberate omission and an oversight look identical otherwise.

---

## The 15 requirements, by family

| Family | Count | Requirements (CMMC L1 ID · NIST 800-171) |
|--------|-------|------------------------------------------|
| Access Control (AC) | 4 | b.1.i · 3.1.1 — b.1.ii · 3.1.2 — b.1.iii · 3.1.20 — b.1.iv · 3.1.22 |
| Identification & Authentication (IA) | 2 | b.1.v · 3.5.1 — b.1.vi · 3.5.2 |
| Media Protection (MP) | 1 | b.1.vii · 3.8.3 |
| Physical Protection (PE) | 2 | b.1.viii · 3.10.1 — b.1.ix · 3.10.3 / 3.10.4 / 3.10.5 |
| System & Communications Protection (SC) | 2 | b.1.x · 3.13.1 — b.1.xi · 3.13.5 |
| System & Information Integrity (SI) | 4 | b.1.xii · 3.14.1 — b.1.xiii · 3.14.2 — b.1.xiv · 3.14.4 — b.1.xv · 3.14.5 |

> **Note on the count.** Earlier CMMC 2.0 material (2021) listed Level 1 as *17 practices* across four separate Physical Protection controls. The current **CMMC Assessment Guide – Level 1, v2.13 (September 2024)** — the version enforceable under 32 CFR § 170.15 since the November 2025 rule — consolidates the former PE practices 3.10.3, 3.10.4, and 3.10.5 into a single requirement, **PE.L1-b.1.ix (Manage Visitors & Physical Access)**. This brings the total to **15 requirements / 58 assessment objectives**. The underlying FAR 52.204-21 safeguarding obligations are unchanged — only the count and structure were consolidated.

> **Note on ID notation.** Each requirement has two equivalent identifiers: the current CMMC format (e.g., `MP.L1-b.1.vii`) and the NIST SP 800-171 number it derives from (e.g., `3.8.3`). This toolkit leads with the CMMC format throughout and carries the NIST number alongside. The Roman numeral is not decorative — it is the FAR 52.204-21(b)(1) subparagraph, so `AC.L1-b.1.iv` is FAR 52.204-21(b)(1)(iv). Useful as a self-check when citing the source.

---

## A note on "Not Applicable"

N/A is rare and risky at Level 1. If an information system processes, stores, or transmits FCI, almost every requirement applies. A defensible N/A is **scope-driven** — the conditions the control governs genuinely don't exist inside the assessment boundary — never a convenience. "We don't do this" is an assumption; "no components within the assessment boundary are publicly accessible" is a determination, and an assessor will ask you to prove the second.

A determination that survives contact with an assessor has three parts, written down before the assessment rather than during it:

1. **The determination** — why the control doesn't apply, tied to the specific boundary condition, and stated in the control's *own vocabulary*. If the requirement says "components," the determination must say components. Narrowing it to "no public web servers" quietly excludes API gateways, status pages, and VPN concentrators — and an assessor will hold you to the wider word.
2. **The boundary logic** — the evidence that the condition holds: what defines the boundary, what's inside it, and how you know nothing inside it is publicly reachable.
3. **The re-evaluation trigger** — the event that voids the determination. Without it, a legitimately inapplicable control becomes silently unmet the day someone stands up a public-facing service, and nobody notices until the next assessment.

Note that evidence changes category under an N/A. For an applicable control, evidence proves *implementation* — policies, configurations, logs. For an N/A control, evidence proves *the condition* — subnet inventory, boundary definition, external scan showing no inbound reachability. Leaving the evidence column empty on an N/A row is how a determination dies under questioning.

This toolkit flags which requirements can legitimately be N/A: realistically only **SC.L1-b.1.xi**, per the Assessment Guide's own example; conditionally **AC.L1-b.1.iv** and the physical-protection requirements for fully remote organizations. Everything else is effectively never N/A. During an assessment an objective assessed N/A is equivalent to MET — which is precisely why each one must be justified in writing and is subject to assessor challenge.

One recurring trap worth naming: **cloud does not remove the boundary — it relocates it.** Teams assume a cloud-hosted service is automatically out of scope, when often the cloud service *is* the publicly accessible component. If the organization operates it, it's in scope wherever it runs. If a third party operates it, that has to be established, not assumed.

---

## Scope & sources

CMMC Level 1 is an annual self-assessment derived from **FAR 52.204-21**, covering 15 requirements that map to a subset of **NIST SP 800-171**. Assessment objectives and methods follow **NIST SP 800-171A** as adopted by the **CMMC Assessment Guide – Level 1 (v2.13)**. Each requirement is scored MET, NOT MET, or NOT APPLICABLE; POA&Ms are not permitted at Level 1. Commercial mappings reference the **AICPA Trust Services Criteria** (SOC 2) and **ISO/IEC 27001:2022** Annex A. All source frameworks are public; this toolkit contains no client data.

*Educational reference, not legal or assessment advice. Confirm requirement applicability and N/A determinations against the current CMMC Assessment Guide and your assessor.*
