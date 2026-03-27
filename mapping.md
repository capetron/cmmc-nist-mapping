# CMMC 2.0 to NIST Complete Control Mapping

This document provides the complete practice-by-practice mapping between CMMC 2.0 Levels 1, 2, and 3 and their source NIST publications: SP 800-171 Rev. 2, SP 800-172, and SP 800-53 Rev. 5.

Last Reviewed: March 2026

---

## CMMC Level 1: FAR 52.204-21 to NIST Mapping (17 Practices)

| CMMC Practice ID | CMMC Practice Description | 800-171 Source | 800-53 Rev. 5 Ancestry | FAR 52.204-21 Reference |
|---|---|---|---|---|
| AC.L1-b.1.i | Limit information system access to authorized users, processes acting on behalf of authorized users, or devices | 3.1.1 | AC-2, AC-3, AC-17 | (b)(1)(i) |
| AC.L1-b.1.ii | Limit information system access to the types of transactions and functions that authorized users are permitted to execute | 3.1.2 | AC-2, AC-3, AC-17 | (b)(1)(ii) |
| AC.L1-b.1.iii | Verify and control/limit connections to and use of external information systems | 3.1.20 | AC-20, AC-20(1) | (b)(1)(iii) |
| AC.L1-b.1.iv | Control information posted or processed on publicly accessible information systems | 3.1.22 | AC-22 | (b)(1)(iv) |
| IA.L1-b.1.v | Identify information system users, processes acting on behalf of users, or devices | 3.5.1 | IA-2, IA-5 | (b)(1)(v) |
| IA.L1-b.1.vi | Authenticate (or verify) the identities of those users, processes, or devices, as a prerequisite to allowing access | 3.5.2 | IA-2, IA-5 | (b)(1)(vi) |
| MP.L1-b.1.vii | Sanitize or destroy information system media containing Federal Contract Information before disposal or release for reuse | 3.8.3 | MP-6 | (b)(1)(vii) |
| PE.L1-b.1.viii | Limit physical access to organizational information systems, equipment, and the respective operating environments to authorized individuals | 3.10.1 | PE-2, PE-6 | (b)(1)(viii) |
| PE.L1-b.1.ix | Escort visitors and monitor visitor activity; maintain audit logs of physical access; and control and manage physical access devices | 3.10.3, 3.10.4, 3.10.5 | PE-2, PE-3, PE-6 | (b)(1)(ix) |
| SC.L1-b.1.x | Monitor, control, and protect organizational communications at the external boundaries of the information systems and at key internal boundaries within the systems | 3.13.1 | SC-7 | (b)(1)(x) |
| SC.L1-b.1.xi | Implement subnetworks for publicly accessible system components that are physically or logically separated from internal networks | 3.13.5 | SC-7 | (b)(1)(xi) |
| SI.L1-b.1.xii | Identify, report, and correct information and information system flaws in a timely manner | 3.14.1 | SI-2 | (b)(1)(xii) |
| SI.L1-b.1.xiii | Provide protection from malicious code at appropriate locations within organizational information systems | 3.14.2 | SI-3 | (b)(1)(xiii) |
| SI.L1-b.1.xiv | Update malicious code protection mechanisms when new releases are available | 3.14.4 | SI-3 | (b)(1)(xiv) |
| SI.L1-b.1.xv | Perform periodic scans of the information system and real-time scans of files from external sources as files are downloaded, opened, or executed | 3.14.5 | SI-3 | (b)(1)(xv) |

Note: The CMMC Final Rule lists 17 Level 1 practices. Two additional practices (PE.L1 visitor controls) are sometimes counted as separate entries depending on how multi-part FAR provisions are parsed.

---

## CMMC Level 2: NIST SP 800-171 Rev. 2 Complete Mapping (110 Practices)

Level 2 maps one-to-one to all 110 NIST SP 800-171 Rev. 2 requirements. Below is the mapping organized by domain.

### Access Control Domain (AC) - 22 Practices

| CMMC Practice | Description | 800-171 | 800-53 | Level 1? |
|---|---|---|---|---|
| AC.L2-3.1.1 | Limit system access to authorized users | 3.1.1 | AC-2, AC-3, AC-17 | Yes |
| AC.L2-3.1.2 | Limit system access to authorized functions | 3.1.2 | AC-2, AC-3, AC-17 | Yes |
| AC.L2-3.1.3 | Control CUI flow per approved authorizations | 3.1.3 | AC-4 | No |
| AC.L2-3.1.4 | Separate duties of individuals | 3.1.4 | AC-5 | No |
| AC.L2-3.1.5 | Employ least privilege | 3.1.5 | AC-6, AC-6(1), AC-6(2), AC-6(5) | No |
| AC.L2-3.1.6 | Use non-privileged accounts for non-security functions | 3.1.6 | AC-6(2) | No |
| AC.L2-3.1.7 | Prevent non-privileged users from executing privileged functions | 3.1.7 | AC-6(9), AC-6(10) | No |
| AC.L2-3.1.8 | Limit unsuccessful logon attempts | 3.1.8 | AC-7 | No |
| AC.L2-3.1.9 | Provide privacy and security notices | 3.1.9 | AC-8 | No |
| AC.L2-3.1.10 | Use session lock with pattern-hiding displays | 3.1.10 | AC-11, AC-11(1) | No |
| AC.L2-3.1.11 | Terminate sessions after defined conditions | 3.1.11 | AC-12 | No |
| AC.L2-3.1.12 | Monitor and control remote access | 3.1.12 | AC-17(1), AC-17(2) | No |
| AC.L2-3.1.13 | Employ cryptographic mechanisms for remote access | 3.1.13 | AC-17(2) | No |
| AC.L2-3.1.14 | Route remote access via managed access control points | 3.1.14 | AC-17(3) | No |
| AC.L2-3.1.15 | Authorize remote execution of privileged commands | 3.1.15 | AC-17(4) | No |
| AC.L2-3.1.16 | Authorize wireless access | 3.1.16 | AC-18, AC-18(1) | No |
| AC.L2-3.1.17 | Protect wireless access with authentication and encryption | 3.1.17 | AC-18(1) | No |
| AC.L2-3.1.18 | Control connection of mobile devices | 3.1.18 | AC-19 | No |
| AC.L2-3.1.19 | Encrypt CUI on mobile devices | 3.1.19 | AC-19(5) | No |
| AC.L2-3.1.20 | Verify and control/limit external connections | 3.1.20 | AC-20, AC-20(1) | Yes |
| AC.L2-3.1.21 | Limit use of portable storage on external systems | 3.1.21 | AC-20(2) | No |
| AC.L2-3.1.22 | Control CUI on publicly accessible systems | 3.1.22 | AC-22 | Yes |

### Awareness and Training Domain (AT) - 3 Practices

| CMMC Practice | Description | 800-171 | 800-53 |
|---|---|---|---|
| AT.L2-3.2.1 | Ensure awareness of security risks | 3.2.1 | AT-2, AT-2(2) |
| AT.L2-3.2.2 | Ensure personnel are trained for security duties | 3.2.2 | AT-3 |
| AT.L2-3.2.3 | Provide insider threat awareness training | 3.2.3 | AT-2(2) |

### Audit and Accountability Domain (AU) - 9 Practices

| CMMC Practice | Description | 800-171 | 800-53 |
|---|---|---|---|
| AU.L2-3.3.1 | Create and retain audit logs | 3.3.1 | AU-2, AU-3, AU-3(1), AU-6, AU-12 |
| AU.L2-3.3.2 | Ensure user actions are uniquely traceable | 3.3.2 | AU-2, AU-3, AU-6, AU-12 |
| AU.L2-3.3.3 | Review and update logged events | 3.3.3 | AU-2(3) |
| AU.L2-3.3.4 | Alert on audit logging process failure | 3.3.4 | AU-5 |
| AU.L2-3.3.5 | Correlate audit records for investigation | 3.3.5 | AU-6(3) |
| AU.L2-3.3.6 | Provide audit record reduction and report generation | 3.3.6 | AU-7 |
| AU.L2-3.3.7 | Synchronize system clocks | 3.3.7 | AU-8, AU-8(1) |
| AU.L2-3.3.8 | Protect audit information from unauthorized access | 3.3.8 | AU-9 |
| AU.L2-3.3.9 | Limit audit logging management to privileged users | 3.3.9 | AU-9(4) |

### Configuration Management Domain (CM) - 9 Practices

| CMMC Practice | Description | 800-171 | 800-53 |
|---|---|---|---|
| CM.L2-3.4.1 | Establish baseline configurations and inventories | 3.4.1 | CM-2, CM-6, CM-8, CM-8(1) |
| CM.L2-3.4.2 | Establish security configuration settings | 3.4.2 | CM-6 |
| CM.L2-3.4.3 | Track, review, approve, and log changes | 3.4.3 | CM-3, CM-3(2) |
| CM.L2-3.4.4 | Analyze security impact of changes | 3.4.4 | CM-4 |
| CM.L2-3.4.5 | Define and enforce access restrictions for changes | 3.4.5 | CM-5 |
| CM.L2-3.4.6 | Employ least functionality | 3.4.6 | CM-7 |
| CM.L2-3.4.7 | Restrict nonessential programs and services | 3.4.7 | CM-7(1), CM-7(2) |
| CM.L2-3.4.8 | Apply deny-by-exception or deny-all policy | 3.4.8 | CM-7(4), CM-7(5) |
| CM.L2-3.4.9 | Control user-installed software | 3.4.9 | CM-11 |

### Identification and Authentication Domain (IA) - 11 Practices

| CMMC Practice | Description | 800-171 | 800-53 | Level 1? |
|---|---|---|---|---|
| IA.L2-3.5.1 | Identify system users and devices | 3.5.1 | IA-2, IA-5 | Yes |
| IA.L2-3.5.2 | Authenticate users and devices | 3.5.2 | IA-2, IA-5 | Yes |
| IA.L2-3.5.3 | Use multifactor authentication | 3.5.3 | IA-2(1), IA-2(2) | No |
| IA.L2-3.5.4 | Employ replay-resistant authentication | 3.5.4 | IA-2(8) | No |
| IA.L2-3.5.5 | Prevent identifier reuse | 3.5.5 | IA-4 | No |
| IA.L2-3.5.6 | Disable identifiers after inactivity | 3.5.6 | IA-4(4) | No |
| IA.L2-3.5.7 | Enforce password complexity | 3.5.7 | IA-5(1) | No |
| IA.L2-3.5.8 | Prohibit password reuse | 3.5.8 | IA-5(1) | No |
| IA.L2-3.5.9 | Allow temporary password use with immediate change | 3.5.9 | IA-5(1) | No |
| IA.L2-3.5.10 | Cryptographically protect passwords | 3.5.10 | IA-5(1) | No |
| IA.L2-3.5.11 | Obscure authentication feedback | 3.5.11 | IA-6 | No |

### Incident Response Domain (IR) - 3 Practices

| CMMC Practice | Description | 800-171 | 800-53 |
|---|---|---|---|
| IR.L2-3.6.1 | Establish incident-handling capability | 3.6.1 | IR-2, IR-4, IR-5, IR-6, IR-7 |
| IR.L2-3.6.2 | Track, document, and report incidents | 3.6.2 | IR-6, IR-6(1) |
| IR.L2-3.6.3 | Test incident response capability | 3.6.3 | IR-3, IR-3(2) |

### Maintenance Domain (MA) - 6 Practices

| CMMC Practice | Description | 800-171 | 800-53 |
|---|---|---|---|
| MA.L2-3.7.1 | Perform system maintenance | 3.7.1 | MA-2 |
| MA.L2-3.7.2 | Control maintenance tools and personnel | 3.7.2 | MA-3, MA-3(1), MA-3(2) |
| MA.L2-3.7.3 | Sanitize equipment for off-site maintenance | 3.7.3 | MA-3(3) |
| MA.L2-3.7.4 | Check media for malicious code before use | 3.7.4 | MA-3(2) |
| MA.L2-3.7.5 | Require MFA for nonlocal maintenance | 3.7.5 | MA-4, MA-4(1) |
| MA.L2-3.7.6 | Supervise unauthorized maintenance personnel | 3.7.6 | MA-5 |

### Media Protection Domain (MP) - 9 Practices

| CMMC Practice | Description | 800-171 | 800-53 | Level 1? |
|---|---|---|---|---|
| MP.L2-3.8.1 | Protect system media containing CUI | 3.8.1 | MP-2, MP-4 | No |
| MP.L2-3.8.2 | Limit access to CUI on system media | 3.8.2 | MP-2 | No |
| MP.L2-3.8.3 | Sanitize or destroy CUI media | 3.8.3 | MP-6 | Yes |
| MP.L2-3.8.4 | Mark media with CUI markings | 3.8.4 | MP-3 | No |
| MP.L2-3.8.5 | Control access to media during transport | 3.8.5 | MP-5, MP-5(4) | No |
| MP.L2-3.8.6 | Encrypt CUI on digital media during transport | 3.8.6 | MP-5(4) | No |
| MP.L2-3.8.7 | Control use of removable media | 3.8.7 | MP-7, MP-7(1) | No |
| MP.L2-3.8.8 | Prohibit portable storage without identifiable owner | 3.8.8 | MP-7(1) | No |
| MP.L2-3.8.9 | Protect confidentiality of backup CUI | 3.8.9 | CP-9 | No |

### Personnel Security Domain (PS) - 2 Practices

| CMMC Practice | Description | 800-171 | 800-53 |
|---|---|---|---|
| PS.L2-3.9.1 | Screen individuals prior to CUI access | 3.9.1 | PS-3, PS-6 |
| PS.L2-3.9.2 | Protect systems during personnel actions | 3.9.2 | PS-4, PS-5 |

### Physical Protection Domain (PE) - 6 Practices

| CMMC Practice | Description | 800-171 | 800-53 | Level 1? |
|---|---|---|---|---|
| PE.L2-3.10.1 | Limit physical access | 3.10.1 | PE-2, PE-6 | Yes |
| PE.L2-3.10.2 | Protect and monitor physical facility | 3.10.2 | PE-2, PE-3, PE-6 | No |
| PE.L2-3.10.3 | Escort visitors | 3.10.3 | PE-2, PE-3 | Yes |
| PE.L2-3.10.4 | Maintain physical access logs | 3.10.4 | PE-2, PE-6 | Yes |
| PE.L2-3.10.5 | Control physical access devices | 3.10.5 | PE-3 | Yes |
| PE.L2-3.10.6 | Safeguard CUI at alternate work sites | 3.10.6 | PE-17 | No |

### Risk Assessment Domain (RA) - 3 Practices

| CMMC Practice | Description | 800-171 | 800-53 |
|---|---|---|---|
| RA.L2-3.11.1 | Periodically assess risk | 3.11.1 | RA-3 |
| RA.L2-3.11.2 | Scan for vulnerabilities | 3.11.2 | RA-5, RA-5(5) |
| RA.L2-3.11.3 | Remediate vulnerabilities | 3.11.3 | RA-5 |

### Security Assessment Domain (CA) - 4 Practices

| CMMC Practice | Description | 800-171 | 800-53 |
|---|---|---|---|
| CA.L2-3.12.1 | Periodically assess security controls | 3.12.1 | CA-2, CA-2(1) |
| CA.L2-3.12.2 | Develop and implement POA&Ms | 3.12.2 | CA-5 |
| CA.L2-3.12.3 | Monitor security controls continuously | 3.12.3 | CA-7 |
| CA.L2-3.12.4 | Develop and maintain SSP | 3.12.4 | PL-2 |

### System and Communications Protection Domain (SC) - 16 Practices

| CMMC Practice | Description | 800-171 | 800-53 | Level 1? |
|---|---|---|---|---|
| SC.L2-3.13.1 | Monitor, control, protect boundary communications | 3.13.1 | SC-7 | Yes |
| SC.L2-3.13.2 | Employ security engineering principles | 3.13.2 | SA-8 | No |
| SC.L2-3.13.3 | Separate user from system management functionality | 3.13.3 | SC-2 | No |
| SC.L2-3.13.4 | Prevent unauthorized info transfer via shared resources | 3.13.4 | SC-4 | No |
| SC.L2-3.13.5 | Implement subnetworks for publicly accessible components | 3.13.5 | SC-7 | Yes |
| SC.L2-3.13.6 | Deny traffic by default, allow by exception | 3.13.6 | SC-7(5) | No |
| SC.L2-3.13.7 | Prevent split tunneling for remote devices | 3.13.7 | SC-7(7) | No |
| SC.L2-3.13.8 | Encrypt CUI in transit | 3.13.8 | SC-8, SC-8(1) | No |
| SC.L2-3.13.9 | Terminate sessions after inactivity | 3.13.9 | SC-10 | No |
| SC.L2-3.13.10 | Manage cryptographic keys | 3.13.10 | SC-12 | No |
| SC.L2-3.13.11 | Employ FIPS-validated cryptography | 3.13.11 | SC-13 | No |
| SC.L2-3.13.12 | Prohibit remote activation of collaborative computing devices | 3.13.12 | SC-15 | No |
| SC.L2-3.13.13 | Control mobile code | 3.13.13 | SC-18 | No |
| SC.L2-3.13.14 | Control VoIP technologies | 3.13.14 | SC-19 | No |
| SC.L2-3.13.15 | Protect session authenticity | 3.13.15 | SC-23 | No |
| SC.L2-3.13.16 | Protect CUI at rest | 3.13.16 | SC-28 | No |

### System and Information Integrity Domain (SI) - 7 Practices

| CMMC Practice | Description | 800-171 | 800-53 | Level 1? |
|---|---|---|---|---|
| SI.L2-3.14.1 | Identify, report, and correct system flaws | 3.14.1 | SI-2 | Yes |
| SI.L2-3.14.2 | Provide malicious code protection | 3.14.2 | SI-3 | Yes |
| SI.L2-3.14.3 | Monitor security alerts and advisories | 3.14.3 | SI-5 | No |
| SI.L2-3.14.4 | Update malicious code protection | 3.14.4 | SI-3 | Yes |
| SI.L2-3.14.5 | Perform periodic and real-time scans | 3.14.5 | SI-3 | Yes |
| SI.L2-3.14.6 | Monitor systems for attacks | 3.14.6 | SI-4, SI-4(4), SI-4(5) | No |
| SI.L2-3.14.7 | Identify unauthorized system use | 3.14.7 | SI-4 | No |

---

## CMMC Level 3: Additional NIST SP 800-172 Requirements (24 Practices)

| 800-172 Req | Description | 800-53 High Ancestry | CMMC Domain |
|---|---|---|---|
| 3.1.1e | Employ dual authorization for critical/sensitive operations | AC-3(2) | AC |
| 3.1.2e | Restrict access from non-organizationally owned systems | AC-17(4) | AC |
| 3.1.3e | Employ automated mechanisms for access enforcement | AC-3(4) | AC |
| 3.4.1e | Establish authoritative source and repository for system components | CM-8(3) | CM |
| 3.4.2e | Employ automated discovery and management of system components | CM-8(2) | CM |
| 3.4.3e | Employ allow-by-exception for software execution | CM-7(5) | CM |
| 3.5.1e | Employ replay-resistant, hardware-based MFA | IA-2(8), IA-2(6) | IA |
| 3.5.2e | Employ automated management of authenticators | IA-5(9) | IA |
| 3.5.3e | Employ identity and credential management for devices | IA-3(1) | IA |
| 3.6.1e | Establish and maintain security operations center | IR-4(11) | IR |
| 3.6.2e | Establish cyber incident response team | IR-10 | IR |
| 3.11.1e | Employ threat intelligence in risk assessments | RA-3(2) | RA |
| 3.11.2e | Conduct cyber threat hunting activities | RA-10 | RA |
| 3.11.3e | Employ advanced automation for security analysis | RA-5(6) | RA |
| 3.13.1e | Employ network isolation techniques | SC-7(29) | SC |
| 3.13.2e | Employ cryptographic mechanisms for CUI in storage | SC-28(1) | SC |
| 3.13.3e | Employ verified boot processes | SC-51 | SC |
| 3.13.4e | Employ physical and logical isolation for CUI | SC-7(21) | SC |
| 3.14.1e | Verify integrity of critical software using root of trust | SI-7(1) | SI |
| 3.14.2e | Monitor organizational systems at increased level of detail | SI-4(10) | SI |
| 3.14.3e | Employ advanced endpoint detection capabilities | SI-4(18) | SI |
| 3.14.4e | Employ cyber deception techniques | SI-20 | SI |
| 3.14.5e | Analyze system behavior to detect lateral movement | SI-4(24) | SI |
| 3.14.6e | Use threat indicator sharing to support threat awareness | SI-5(1) | SI |

---

## DFARS Clause Cross-Reference

| DFARS Clause | What It Requires | CMMC Level Connection |
|---|---|---|
| 48 CFR 52.204-21 | Basic safeguarding of FCI (15 requirements) | CMMC Level 1 foundation |
| 252.204-7012 | Implement NIST SP 800-171 for CUI; 72-hour incident reporting to DC3 | CMMC Level 2 foundation |
| 252.204-7019 | Self-assessment per NIST SP 800-171 DoD Assessment Methodology; post score to SPRS | CMMC Level 2 pre-assessment |
| 252.204-7020 | DoD may conduct Medium or High NIST assessments | CMMC Level 2 government oversight |
| 252.204-7021 | CMMC certification required at specified level as condition of contract award | CMMC implementation clause |

---

## Sources

- [32 CFR Part 170 (CMMC Final Rule)](https://www.ecfr.gov/current/title-32/subtitle-A/chapter-I/subchapter-D/part-170)
- [NIST SP 800-171 Rev. 2](https://csrc.nist.gov/publications/detail/sp/800-171/rev-2/final)
- [NIST SP 800-172](https://csrc.nist.gov/publications/detail/sp/800-172/final)
- [NIST SP 800-53 Rev. 5](https://csrc.nist.gov/publications/detail/sp/800-53/rev-5/final)
- [DFARS PGI 204.73](https://www.acq.osd.mil/dpap/dars/dfars/html/current/204_73.htm)
- [FAR 52.204-21](https://www.acquisition.gov/far/52.204-21)

---

Maintained by [Petronella Technology Group, Inc.](https://petronellatech.com) | Call 919-348-4912 for CMMC assessment
