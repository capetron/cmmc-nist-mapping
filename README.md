# CMMC to NIST Control Mapping

A comprehensive mapping between the Cybersecurity Maturity Model Certification (CMMC) 2.0 and the NIST Special Publications that form its foundation: SP 800-171 Rev. 2, SP 800-172, and SP 800-53 Rev. 5. This repository details how CMMC Levels 1, 2, and 3 trace to specific NIST controls, covers all 14 CMMC domains, and clarifies the DFARS clauses that make CMMC a contractual obligation for defense contractors.

**Full reference page:** [https://petronellatech.com/compliance/cmmc-nist-mapping/](https://petronellatech.com/compliance/cmmc-nist-mapping/)

Last Reviewed: March 2026

---

## Table of Contents

1. [What Is CMMC 2.0?](#what-is-cmmc-20)
2. [The NIST Foundation of CMMC](#the-nist-foundation-of-cmmc)
3. [CMMC Levels and Their NIST Sources](#cmmc-levels-and-their-nist-sources)
4. [The 14 CMMC Domains](#the-14-cmmc-domains)
5. [Level 1 to NIST Mapping](#level-1-to-nist-mapping)
6. [Level 2 to NIST 800-171 Mapping](#level-2-to-nist-800-171-mapping)
7. [Level 3 to NIST 800-172 Mapping](#level-3-to-nist-800-172-mapping)
8. [DFARS Clauses and Their CMMC Connections](#dfars-clauses-and-their-cmmc-connections)
9. [The 800-53 Ancestry](#the-800-53-ancestry)
10. [Assessment Types by Level](#assessment-types-by-level)
11. [SPRS Scoring and CMMC Readiness](#sprs-scoring-and-cmmc-readiness)
12. [Domain-by-Domain Breakdown](#domain-by-domain-breakdown)
13. [Practical Implementation Strategy](#practical-implementation-strategy)
14. [Common Pitfalls in CMMC-NIST Alignment](#common-pitfalls-in-cmmc-nist-alignment)
15. [Timeline and Phased Rollout](#timeline-and-phased-rollout)
16. [About PTG](#about-ptg)
17. [License](#license)

---

## What Is CMMC 2.0?

The Cybersecurity Maturity Model Certification (CMMC) 2.0 is the Department of Defense's verification mechanism for ensuring that defense contractors adequately protect Federal Contract Information (FCI) and Controlled Unclassified Information (CUI). Published as 32 CFR Part 170, CMMC replaced the self-attestation model with a tiered certification system that ranges from annual self-assessment (Level 1) to government-led assessment (Level 3).

CMMC 2.0 simplified the original CMMC 1.0 model from five levels to three:

| CMMC Level | Information Protected | Assessment Type | NIST Source |
|---|---|---|---|
| Level 1 | Federal Contract Information (FCI) | Annual self-assessment | FAR 52.204-21 (15 requirements, derived from 800-171 basic controls) |
| Level 2 | Controlled Unclassified Information (CUI) | Triennial third-party assessment (C3PAO) or self-assessment for select programs | NIST SP 800-171 Rev. 2 (110 requirements) |
| Level 3 | CUI on highest-priority programs | Government-led assessment (DIBCAC) | NIST SP 800-172 (selected enhanced requirements) plus all of 800-171 |

Source: [32 CFR Part 170, CMMC Program Final Rule](https://www.ecfr.gov/current/title-32/subtitle-A/chapter-I/subchapter-D/part-170)

## The NIST Foundation of CMMC

CMMC did not invent new security requirements. Every CMMC practice traces directly to an existing NIST publication:

- **Level 1 practices** come from FAR 52.204-21, "Basic Safeguarding of Covered Contractor Information Systems," which codifies 15 basic safeguarding requirements. These 15 requirements are themselves derived from NIST SP 800-171 basic security requirements.
- **Level 2 practices** are a one-to-one mapping to all 110 security requirements in NIST SP 800-171 Rev. 2. There are no additional practices. CMMC Level 2 IS 800-171.
- **Level 3 practices** add 24 selected requirements from NIST SP 800-172, "Enhanced Security Requirements for Protecting Controlled Unclassified Information." 800-172 itself derives from the 800-53 High baseline.

This means the complete NIST lineage of CMMC is: 800-53 Rev. 5 (master catalog) to 800-171 Rev. 2 (CUI subset) to CMMC Level 2 (certification wrapper), with 800-172 extending into 800-53 High territory for Level 3.

## CMMC Levels and Their NIST Sources

### Level 1: Basic Safeguarding (17 Practices)

Level 1 contains 17 practices mapped from FAR 52.204-21. These correspond to a subset of 800-171 basic requirements:

| Practice ID | Practice Description | 800-171 Source | 800-53 Ancestry |
|---|---|---|---|
| AC.L1-3.1.1 | Limit system access to authorized users | 3.1.1 | AC-2, AC-3, AC-17 |
| AC.L1-3.1.2 | Limit system access to authorized functions | 3.1.2 | AC-2, AC-3, AC-17 |
| AC.L1-3.1.20 | Verify and control external connections | 3.1.20 | AC-20 |
| AC.L1-3.1.22 | Control publicly accessible information | 3.1.22 | AC-22 |
| IA.L1-3.5.1 | Identify system users | 3.5.1 | IA-2, IA-5 |
| IA.L1-3.5.2 | Authenticate users | 3.5.2 | IA-2, IA-5 |
| MP.L1-3.8.3 | Sanitize or destroy media | 3.8.3 | MP-6 |
| PE.L1-3.10.1 | Limit physical access | 3.10.1 | PE-2, PE-6 |
| PE.L1-3.10.3 | Escort visitors | 3.10.3 | PE-2, PE-6 |
| PE.L1-3.10.4 | Maintain physical access logs | 3.10.4 | PE-2, PE-6 |
| PE.L1-3.10.5 | Manage physical access devices | 3.10.5 | PE-3 |
| SC.L1-3.13.1 | Monitor communications at boundaries | 3.13.1 | SC-7 |
| SC.L1-3.13.5 | Implement subnetworks for publicly accessible systems | 3.13.5 | SC-7 |
| SI.L1-3.14.1 | Identify and correct system flaws | 3.14.1 | SI-2 |
| SI.L1-3.14.2 | Provide malicious code protection | 3.14.2 | SI-3 |
| SI.L1-3.14.4 | Update malicious code protection | 3.14.4 | SI-3 |
| SI.L1-3.14.5 | Perform system and file scans | 3.14.5 | SI-3 |

### Level 2: CUI Protection (110 Practices)

Level 2 maps one-to-one to all 110 NIST SP 800-171 Rev. 2 security requirements. No additional practices, no removed practices. The complete mapping is available in [mapping.md](mapping.md).

### Level 3: Enhanced CUI Protection (110 + 24 Practices)

Level 3 includes all 110 Level 2 practices plus 24 selected requirements from NIST SP 800-172. The 24 additional requirements address advanced threats such as APTs:

| 800-172 Requirement | Description | 800-53 High Ancestry |
|---|---|---|
| 3.1.1e | Employ dual authorization for critical operations | AC-3(2) |
| 3.1.2e | Restrict access to systems from external networks | AC-17(4) |
| 3.1.3e | Employ automated mechanisms to enforce access restrictions | AC-3(4) |
| 3.4.1e | Establish and maintain an authoritative source for system components | CM-8(3) |
| 3.4.2e | Employ automated discovery of system components | CM-8(2) |
| 3.5.1e | Employ replay-resistant authentication | IA-2(8) |
| 3.5.3e | Employ automated tools to manage authenticators | IA-5(9) |
| 3.6.1e | Establish security operations center capability | IR-4(11) |
| 3.6.2e | Establish and maintain cyber incident response team | IR-10 |
| 3.11.1e | Employ threat intelligence for risk decisions | RA-3(2) |
| 3.11.2e | Conduct cyber threat hunting | RA-10 |
| 3.13.1e | Employ isolation techniques in network architecture | SC-7(29) |
| 3.13.4e | Employ cryptographic mechanisms to prevent unauthorized disclosure | SC-28(1) |
| 3.14.1e | Verify integrity of security-critical software | SI-7(1) |
| 3.14.2e | Monitor organizational systems for security-relevant events | SI-4(10) |
| 3.14.3e | Employ advanced detection capabilities | SI-4(18) |

Source: [NIST SP 800-172](https://csrc.nist.gov/publications/detail/sp/800-172/final)

## DFARS Clauses and Their CMMC Connections

Multiple DFARS clauses work together to establish CMMC as a contractual requirement:

| DFARS Clause | Purpose | CMMC Connection |
|---|---|---|
| 252.204-7012 | Safeguarding Covered Defense Information | Requires 800-171 implementation; the original mandate that CMMC now verifies |
| 252.204-7019 | Notice of NIST SP 800-171 Assessment Requirements | Requires self-assessment score posted to SPRS; precursor to CMMC self-assessment |
| 252.204-7020 | NIST SP 800-171 DoD Assessment Requirements | Allows government Medium/High assessments; precursor to CMMC C3PAO/DIBCAC assessments |
| 252.204-7021 | CMMC Requirements | The actual CMMC clause requiring certification at specified level as condition of contract award |
| 48 CFR 52.204-21 | Basic Safeguarding | FAR clause requiring the 15 basic safeguarding requirements; foundation for CMMC Level 1 |

Source: [DFARS PGI 204.73](https://www.acq.osd.mil/dpap/dars/dfars/html/current/204_73.htm)

## The 800-53 Ancestry

Every CMMC practice ultimately traces back to NIST SP 800-53 Rev. 5. The lineage is:

```
800-53 Rev. 5 (1,000+ controls, 20 families)
    |
    v [Tailored for nonfederal CUI]
800-171 Rev. 2 (110 requirements, 14 families)
    |
    v [Wrapped in certification framework]
CMMC Level 2 (110 practices, 14 domains)
    |
    + [Enhanced requirements from 800-53 High]
    v
800-172 (35 enhanced requirements)
    |
    v [24 selected for CMMC Level 3]
CMMC Level 3 (134 total practices)
```

This lineage matters because organizations implementing 800-53 Moderate can demonstrate CMMC Level 2 compliance with minimal additional effort. Organizations already FedRAMP authorized at Moderate or High have implemented controls that far exceed CMMC Level 2 requirements.

## Assessment Types by Level

| Aspect | Level 1 | Level 2 | Level 3 |
|---|---|---|---|
| Assessment Body | Self | C3PAO (or self for select programs) | DIBCAC (Government) |
| Frequency | Annual | Triennial | Triennial |
| POA&M Allowed | Yes, 180-day closeout | Yes, 180-day closeout | Limited |
| Conditional Status | N/A | Yes, if POA&Ms exist | No |
| Score Submission | SPRS | SPRS + eMASS | SPRS + eMASS |
| Cost (Typical SMB) | $5,000 to $15,000 internal | $30,000 to $100,000+ (assessment fee + remediation) | $100,000 to $500,000+ |

## SPRS Scoring and CMMC Readiness

The Supplier Performance Risk System (SPRS) score provides a numerical assessment of 800-171 implementation. Every 800-171 requirement carries a weighted value; total possible score is 110. The weighting was determined by DoD based on each control's criticality:

- A score of 110 means all 110 requirements are fully implemented.
- A score of -203 means no requirements are implemented (each unimplemented requirement subtracts its weighted value).
- Most organizations score between 50 and 90 before formal remediation.

SPRS scores map to CMMC readiness:
- **Score 110**: Fully ready for Level 2 assessment
- **Score 80-109**: Close to ready; POA&Ms needed for gaps
- **Score 50-79**: Significant work remaining; 6-12 months remediation typical
- **Score below 50**: Major gaps; 12-18+ months remediation typical

Calculate your score: [PTG SPRS Calculator](https://petronellatech.com/tools/sprs-calculator/)

## Domain-by-Domain Breakdown

The 14 CMMC domains map directly to the 14 NIST SP 800-171 families:

| CMMC Domain | 800-171 Family | L1 Practices | L2 Practices | Key Controls |
|---|---|---|---|---|
| Access Control (AC) | 3.1 | 4 | 22 | Account management, least privilege, remote access, session control |
| Awareness and Training (AT) | 3.2 | 0 | 3 | Security awareness, role-based training, insider threat |
| Audit and Accountability (AU) | 3.3 | 0 | 9 | Audit logging, correlation, retention, protection of audit info |
| Configuration Management (CM) | 3.4 | 0 | 9 | Baseline configs, change control, least functionality, software restrictions |
| Identification and Authentication (IA) | 3.5 | 2 | 11 | MFA, password management, authenticator management, device auth |
| Incident Response (IR) | 3.6 | 0 | 3 | IR capability, reporting, testing |
| Maintenance (MA) | 3.7 | 0 | 6 | Controlled maintenance, tools, remote maintenance, personnel |
| Media Protection (MP) | 3.8 | 1 | 9 | Media access, marking, storage, transport, sanitization, CUI marking |
| Personnel Security (PS) | 3.9 | 0 | 2 | Screening, personnel actions during transfer/termination |
| Physical Protection (PE) | 3.10 | 4 | 6 | Access authorization, monitoring, visitor control, access logs |
| Risk Assessment (RA) | 3.11 | 0 | 3 | Risk assessments, vulnerability scanning, remediation |
| Security Assessment (CA) | 3.12 | 0 | 4 | Periodic assessment, POA&Ms, monitoring, SSP |
| System and Communications Protection (SC) | 3.13 | 2 | 16 | Boundary protection, FIPS crypto, collaborative computing, mobile code |
| System and Information Integrity (SI) | 3.14 | 4 | 7 | Flaw remediation, malicious code, monitoring, alerts, update management |
| **Totals** | | **17** | **110** | |

## Practical Implementation Strategy

1. **Score your current state.** Use the SPRS calculator to establish a baseline score. This determines your gap size and remediation timeline.

2. **Implement Level 1 first.** The 17 Level 1 practices represent basic cyber hygiene. If you cannot meet Level 1, you are at serious risk regardless of contractual requirements.

3. **Build to Level 2 by domain priority.** Focus first on Access Control (22 practices, highest count), then System and Communications Protection (16 practices), then Identification and Authentication (11 practices). These three domains contain 49 of the 110 practices.

4. **Document as you implement.** CMMC assessors evaluate documentation as heavily as technical controls. Every practice needs a policy, a procedure, and evidence of execution. Assessors check for "implemented, not just documented."

5. **Use 800-53 as your reference implementation.** When 800-171 is ambiguous about what a requirement means in practice, read the parent 800-53 control and its supplemental guidance. 800-53 provides significantly more implementation detail.

6. **Plan for Level 3 if you handle critical CUI.** Level 3 requires a Security Operations Center, cyber threat hunting, and hardware-rooted trust. These capabilities take 12-24 months to build.

## Common Pitfalls in CMMC-NIST Alignment

1. **Assuming CMMC adds requirements beyond NIST.** It does not. CMMC Level 2 is exactly 800-171. The "maturity" processes from CMMC 1.0 were removed in 2.0.

2. **Ignoring flow-down requirements.** If you are a prime contractor, your subcontractors who handle CUI must also meet CMMC Level 2. This is a DFARS flow-down requirement under 252.204-7012.

3. **Using Rev. 3 when CMMC references Rev. 2.** CMMC 2.0 currently references 800-171 Rev. 2. Organizations should implement against Rev. 2 for certification while monitoring DoD announcements about Rev. 3 adoption.

4. **Treating POA&Ms as permanent solutions.** CMMC allows POA&Ms at Level 2 with a 180-day closeout window. But too many open POA&Ms (especially on high-weighted controls) can prevent conditional certification.

5. **Underestimating the SSP requirement.** Although 800-171 technically excludes PL-2 (System Security Plan) as a FED control, DFARS 252.204-7012(c)(2) explicitly requires an SSP. CMMC assessors will ask for it.

## Timeline and Phased Rollout

CMMC 2.0 is rolling out in four phases beginning in 2025:

| Phase | Timeframe | Requirement |
|---|---|---|
| Phase 1 | 2025 Q1+ | Level 1 self-assessment or Level 2 self-assessment as condition of contract award |
| Phase 2 | 2025 Q3+ | Level 2 C3PAO assessment required for applicable contracts |
| Phase 3 | 2026+ | Level 2 required for all contracts with CUI; Level 3 for select programs |
| Phase 4 | 2027+ | Full implementation across all applicable DoD contracts |

Organizations should not wait. Assessment backlogs at C3PAOs are already significant, and remediation typically takes 6-12 months for Level 2 and 12-24 months for Level 3.

## About PTG

This repository is maintained by **Petronella Technology Group, Inc. (PTG)**, a cybersecurity, compliance, and AI services firm headquartered in Raleigh, North Carolina.

**Craig Petronella**, PTG's founder, brings the following credentials to compliance advisory:

- CMMC Registered Practitioner (RP)
- Licensed Digital Forensic Examiner #604180
- Cisco CCNA and CWNE certifications
- MIT Artificial Intelligence Certificate
- Amazon #1 Best-Selling Author of 14+ cybersecurity books
- 23+ years of cybersecurity experience

**What makes PTG different:**

- **AI-Powered Compliance.** PTG uses its own private AI fleet, including on-premise LLMs and custom GPU infrastructure, to accelerate compliance assessments, automate control mapping, and continuously monitor security posture. No other firm in the Triangle has this capability.
- **Patented Technology Stack.** PTG's proprietary and patented security tools automate what competitors do manually.
- **Licensed Digital Forensic Examiner.** When compliance fails and a breach occurs, PTG has the forensic expertise to investigate, preserve evidence, and support legal proceedings.
- **AI + Cybersecurity Combined.** PTG is one of the only firms combining AI development (custom AI agents, private LLMs, GPU hosting) with cybersecurity and compliance.
- **SMB Focus.** PTG makes enterprise-grade compliance accessible to small and mid-size businesses.

**Contact PTG:**

- Phone: 919-348-4912
- Web: [https://petronellatech.com](https://petronellatech.com)
- Compliance Services: [https://petronellatech.com/compliance/packages/](https://petronellatech.com/compliance/packages/)
- CMMC Hub: [https://petronellatech.com/compliance/cmmc/](https://petronellatech.com/compliance/cmmc/)
- NIST Hub: [https://petronellatech.com/nist/](https://petronellatech.com/nist/)
- SPRS Calculator: [https://petronellatech.com/tools/sprs-calculator/](https://petronellatech.com/tools/sprs-calculator/)

**Address:** 5540 Centerview Dr. Suite 200, Raleigh, NC 27606

Call 919-348-4912 or visit [petronellatech.com/compliance/packages/](https://petronellatech.com/compliance/packages/) to schedule a free compliance assessment.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
