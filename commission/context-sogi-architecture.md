# Context: Washington SOGI Data Architecture and the Oregon Comparison

> This file is reference context for `commission/plan.md`. Load it on demand — not at session start.

## What this is, in one paragraph

Washington has assembled a strong but fragmented set of SOGI (Sexual Orientation and Gender Identity) data collection requirements across health, public health surveillance, youth surveys, and Medicaid. What it does not have is a statewide, cross-agency standard with a centralized confidential intake registry that binds every state-funded program. Oregon built that with HB 3159 in 2021. The practical result is that Washington can describe LGBTQ+ disparities in some domains (hospital encounters, youth, BRFSS-surveyed adults, trans Medicaid enrollees) but is structurally blind in the systems where over-representation is most consequential: child welfare, adult homelessness, the Medicaid front door, unemployment insurance, and the basic-needs safety net.

---

## Why SOGI data infrastructure matters

Disparities that are not measured cannot be governed. For LGBTQ+ populations, this is not abstract: every credible national study shows over-representation in foster care, youth and adult homelessness, behavioral health crises, and economic insecurity. But "national estimates" are exactly that — estimates. A state cannot allocate resources, evaluate programs, or hold agencies accountable without its own administrative data. SOGI in administrative systems is the difference between policy that can see the people it is meant to serve and policy that has to guess.

The structural argument is post-partisan: this is governance-as-integrity. You cannot evaluate program effectiveness for a population you cannot count. Privacy protection is a design problem, not a reason not to build — Oregon's model demonstrates that confidentiality and aggregation safeguards are compatible with statewide collection.

---

## The Oregon model: HB 3159 (2021)

Oregon's HB 3159 is the reference architecture. Key features:

- **Combined REALD + SOGI standard.** REALD = Race, Ethnicity, Language, Disability. SOGI = Sexual Orientation, Gender Identity. One unified set of standardized questions, codified in Oregon Administrative Rules (permanent rules adopted July 2024).
- **Centralized confidential Registry.** A single intake hub for data submissions from providers, insurers, and Coordinated Care Organizations (CCOs). Oregon explicitly designed it to receive data via EHR integration, QR-code-driven self-survey, or a direct-to-individual portal.
- **Repository for storage and quality processing.** Distinct from the Registry; longitudinal, supports data quality work.
- **Aggregate-only public release.** Statutorily protected confidentiality; raw records are not released.
- **Binding application.** Providers, insurers, and CCOs are required to submit annually for all patients/members once the Registry is operational. OHA has compliance monitoring authority and discretionary civil penalty authority.
- **Community grant program.** Funds community-based organizations serving tribal, BIPOC, LGBTQ+, disability, and limited-English communities to collect and report data safely. Initial funding round expected Spring 2025.
- **Dedicated infrastructure.** HB 3159 came with appropriated staffing across OHA's Equity & Inclusion Division, Office of Information Services, Health Policy and Analytics Division, and Health Systems Division.

The architectural insight: **Oregon built the plumbing first** — the standard, the registry, the rules, the funding — and then turned on the requirement. Washington has built requirements piecemeal in individual statutes, each with its own intake path.

---

## What Washington already has

**Hospital discharge data — E2SHB 1272 / RCW 43.70.052.** Effective January 1, 2023, hospitals report SOGI in patient discharge data submitted to DOH's CHARS system. Closest WA analog to the Oregon model — but covers only hospital encounters, only at discharge.

**BRFSS SOGI module.** Sample-based telephone survey data. Useful for population-level prevalence, not for measuring disparities in service delivery.

**Healthy Youth Survey.** Biennial, ~217,000 students. Best-in-class for youth-level data on LGBTQ+ outcomes in education, behavioral health, substance use. Limitation: in-school students only.

**Apple Health Transhealth records.** HCA maintains gender-identity records for trans members in connection with gender-affirming care utilization. Not a population denominator; not a SOGI standard at intake.

**Office of Equity disaggregation mandate — RCW 43.06D.** Authority to "establish standards for the collection, analysis, and reporting of disaggregated data." The authority exists. Infrastructure to operationalize it for SOGI does not.

---

## The five gaps

### 1. DCYF FamLink (child welfare)
FamLink is the system of record for foster care, CPS, and in-home services. National research finds LGBTQ+ youth over-represented in foster care by ~2–3x (higher for trans/GE youth). Without SOGI in FamLink, WA cannot quantify over-representation, measure differential outcomes, evaluate placement quality, or hold DCYF accountable on equity goals. The Healthy Youth Survey cannot help — foster youth are a small subgroup who often miss school-based administration.

### 2. Balance-of-State HMIS (adult homelessness)
OHY-funded providers have SOGI requirements; the broader Balance-of-State CoC HMIS covering most adult homeless services outside King/Pierce does not. LGBTQ+ adults — especially trans adults — experience homelessness at substantially higher rates. Adult homelessness is the larger system and the larger blind spot.

### 3. Apple Health single streamlined application (Medicaid intake)
Downstream data exists (Transhealth records, claims). The population denominator at intake does not capture SOGI. HCA can describe utilization among trans members it has identified, but cannot describe access, enrollment friction, or churn for LGBTQ+ Washingtonians as a population.

### 4. ESD / Unemployment Insurance claims
Labor market discrimination against LGBTQ+ workers (especially trans) is well-documented. Without SOGI in UI data, WA cannot evaluate differential access, benefit duration, return-to-work outcomes, or industry-level patterns.

### 5. DSHS ESA intake (basic-needs safety net)
ESA runs TANF, Basic Food, ABD, and refugee/working family support. This is where economic precarity is measured. ESA can describe its caseload by race and household composition; it cannot describe it by SOGI. Adding SOGI here would most directly allow WA to characterize LGBTQ+ economic vulnerability in the populations the safety net is meant to catch.

---

## The architectural difference

Washington has built **requirements**. Oregon has built **infrastructure**. Three features WA lacks:

1. **A single standardized question set** binding across agencies. WA's hospital SOGI fields, HCA's gender-identity capture, OHY's HMIS questions, and HYS items are all different.
2. **A centralized confidential Registry** as the intake hub. WA has multiple intake systems each managing its own SOGI data with its own protections.
3. **Statutory binding application across every state-funded program.** WA binds hospitals and survey programs. Oregon binds providers, insurers, and CCOs — extensible to any state-funded service.

---

## Three pathways forward

**Incremental.** Add SOGI requirements to specific systems one at a time, starting with DCYF FamLink (highest human stakes, lowest data overhead). This is the path WA is currently on.

**Office-of-Equity-led standardization.** Use existing RCW 43.06D authority to publish a binding statewide REALD+SOGI standard and require agency adoption via executive order or budget proviso. Achieves question-set unification without new statute; stops short of a centralized Registry.

**Washington HB 3159-equivalent.** New statute creating a centralized confidential Registry, unified standard, binding application for providers/insurers/MCOs/state-funded programs, aggregate-only release, dedicated infrastructure within Office of Equity or DOH, and a community grant program. The structural fix. Closes all five gaps. Requires legislative champion, appropriation, and likely multi-session timeline. Oregon's bill passed in 2021; permanent administrative rules adopted July 2024.

**Commission leverage is strongest in pathways 1 and 2.** Pathway 3 requires a legislative champion.
