## CMMC Level 1 Readiness Toolkit

A practitioner's reference library for the **15 requirements of CMMC Level 1** (58 assessment objectives) — the cybersecurity baseline that protects **Federal Contract Information (FCI)** for organizations in the U.S. Defense Industrial Base. For each requirement, the toolkit answers the questions a small business (and its assessor) actually asks: *who owns it, what it means, how it's audited, what evidence proves it, what to ask, and when it doesn't apply* — plus how each requirement maps to the commercial frameworks (**SOC 2** and **ISO 27001:2022**) those same businesses often need next.

> **Author:** Johnbosco Ibeneme · **Focus:** Governance, Risk & Compliance (GRC) · CMMC / NIST 800-171 / SOC 2 / ISO 27001

---

## Why this exists

Most CMMC tooling tells you *whether* a requirement is met. It rarely tells a non-expert *how to know*. This toolkit closes that gap with a single, repeatable structure applied consistently across all 15 Level 1 requirements, so a small business can self-assess honestly and an assessor can follow the reasoning.

It also does something most CMMC references don't: it **maps every requirement to its SOC 2 and ISO 27001 equivalents.** Federal and commercial compliance are the same discipline in different dialects — a large share of the substance overlaps. Showing that overlap turns "we did CMMC" into "we have a control baseline that ports to the commercial audits our customers ask for."

---

## The structure (every requirement follows the same 8 sections)

| # | Section | What it answers |
|---|---------|-----------------|
| 0 | **Identity** | Practice statement, level, and the formal assessment objectives ([a], [b], …) |
| 1 | **Intent** | What the requirement is really asking for, in plain language |
| 2 | **Ownership** | Who is *Responsible* (does it) vs *Accountable* (owns the outcome) |
| 3 | **Assessment** | How an assessor audits it — Examine / Interview / Test |
| 4 | **Evidence** | The artifacts to have ready (final, approved — drafts are not valid evidence) |
| 5 | **Customer Questions** | Tiered questions to determine status (scope → implementation → evidence) |
| 6 | **Not Applicable** | Honest N/A eligibility + defensible verbiage |
| 7 | **Commercial Mapping** | SOC 2 (TSC) and ISO 27001:2022 Annex A equivalents |

---

## What's in this repo

- **`CMMC_L1_Master_Readiness_Library.xlsx`** — all 15 requirements in one workbook, every section as a column. The master reference. IDs lead with the current CMMC L1 format (e.g., `MP.L1-b.1.vii`) with the NIST 800-171 number (e.g., `3.8.3`) in the mapping column.
- **`deep-dives/`** — full-page worked sheets for the requirements with real nuance:
  - **Media Disposal (MP.L1-b.1.vii)** — the template exemplar, showing all 8 sections worked end to end.
  - *More deep-dives in progress* — Public-Access System Separation (SC.L1-b.1.xi, the realistic N/A case) and Control Public Information (AC.L1-b.1.iv, a conditional N/A case) are next.
- **`README.md`** — this file.

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

> **Note on ID notation.** Each requirement has two equivalent identifiers: the current CMMC format (e.g., `MP.L1-b.1.vii`) and the NIST SP 800-171 number it derives from (e.g., `3.8.3`). The workbook and README lead with the current CMMC format; some deep-dive sheets use the composite `MP.L1-3.8.3` style. Both point to the same control — the notations are interchangeable, not different requirements.

---

## A note on "Not Applicable"

N/A is rare and risky at Level 1. If an information system processes, stores, or transmits FCI, almost every requirement applies. A defensible N/A is **scope-driven** — the capability genuinely doesn't exist in the environment — never a convenience. This toolkit flags exactly which requirements can legitimately be N/A (realistically, only **SC.L1-b.1.xi**, per the Assessment Guide's own example; conditionally, **AC.L1-b.1.iv** and the physical-protection requirements for fully remote organizations) and provides defensible verbiage for each. During an assessment, an objective assessed N/A is equivalent to MET — but each N/A must be justified in writing and is subject to assessor challenge. Making N/A *hard to claim and easy to justify* is what keeps a self-assessment credible.

---

## Scope & sources

CMMC Level 1 is an annual self-assessment derived from **FAR 52.204-21**, covering 15 requirements that map to a subset of **NIST SP 800-171**. Assessment objectives and methods follow **NIST SP 800-171A** as adopted by the **CMMC Assessment Guide – Level 1 (v2.13)**. Each requirement is scored MET, NOT MET, or NOT APPLICABLE; POA&Ms are not permitted at Level 1. Commercial mappings reference the **AICPA Trust Services Criteria** (SOC 2) and **ISO/IEC 27001:2022** Annex A. All source frameworks are public; this toolkit contains no client data.

*Educational reference, not legal or assessment advice. Confirm requirement applicability and N/A determinations against the current CMMC Assessment Guide and your assessor.*
