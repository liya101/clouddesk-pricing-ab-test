# CloudDesk — Pricing Page A/B Test

A three-part case study designing, analysing, and recommending on a (synthetic) B2B SaaS pricing page redesign experiment.

> **TL;DR** — A 4-week test of an annual-default pricing page lifted annual signup share by **+8.3 percentage points** (19.5% → 27.8%) but breached both pre-registered guardrails: signup conversion dropped −0.49pp and revenue per visitor dropped −4.5%. The test "failed" overall, but **subgroup analysis revealed the failure is sharply concentrated in companies with <50 employees**. For 50+ companies, the redesign performs cleanly. **Recommendation: segmented rollout — ship for 50+, iterate the design for SMB.**

📄 **Full case study writeup:** https://www.notion.so/CloudDesk-Pricing-Page-A-B-Test-350658b8997e81368b70c843014b343d?source=copy_link

---

## The problem

CloudDesk, a B2B SaaS company, wants to push more customers to annual contracts (which retain better and produce predictable revenue). The proposed change: redesign the pricing page so the annual price is the headline ("$9.60/user/month, billed annually") with a "Save 20%" badge.

The hypothesis: shifting the default to annual will lift annual signup share, **without** significantly hurting overall signup conversion.

This case study covers all three acts:

1. **Test design** (pre-launch) — primary metric, guardrails, sample size, pre-registered subgroups, decision criteria
2. **Test analysis** (post-launch) — integrity checks, primary metric, guardrails, subgroup analysis
3. **Recommendation** — ship/kill/iterate/follow-up, with explicit reasoning grounded in pre-registered criteria

---

## Why this case study

A/B test design is the most-asked, least-prepared topic in product analyst interviews. Most portfolio projects show "I analysed an A/B test result." This one shows the full lifecycle:

- A power calculation with explicit MDE reasoning
- Pre-registered subgroups and decision criteria committed *before* seeing the results
- A trade-off that doesn't resolve cleanly — both guardrails breached but subgroups tell a more nuanced story
- A recommendation that updates from "blanket iterate" to "segmented rollout" based on the data


---

## Key findings

- **Primary metric:** annual share of signups lifted from 19.5% to 27.8% — a **+8.3pp lift** (p ≈ 0). Well above the 3pp shipping threshold and 5pp MDE.
- **Guardrail 1 — Signup conversion:** dropped from 4.71% to 4.22% — a **−0.49pp drop** (p ≈ 0). Breaches the −0.3pp pre-registered tolerance.
- **Guardrail 2 — Revenue per visitor:** dropped from $7.95 to $7.60 — a **−4.5% relative decline** (p = 0.04, borderline). Breaches the "flat or positive" pre-registered threshold.
- **Subgroup story (the most important finding):** the damage concentrates entirely in <50 employee companies. For 50+ segments, revenue is roughly neutral (+0.8%) with strong annual lift (+8.7pp to +9.9pp).

---

## Recommendation

**Iterate — but with a segmented launch path:**

1. **Ship the redesign immediately to 50+ employee visitors.** Strong annual lift, no measurable revenue cost.
2. **Iterate the design for <50 employee visitors.** Specifically test a softer annual presentation (e.g. show monthly equivalent prominently alongside annual headline).
3. **Add long-term retention measurement** to any future iteration — first-year revenue undersells annual customer value.


---

## Repo structure
