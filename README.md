# CMMC Compliance Toolkit | By Petronella Technology Group

**The most comprehensive open-source CMMC 2.0 compliance resource on GitHub.** Free checklists, self-assessment templates, SSP outlines, POA&M templates, and audit scripts to help defense contractors achieve CMMC certification.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Maintained by PTG](https://img.shields.io/badge/Maintained%20by-Petronella%20Technology%20Group-orange)](https://petronellatech.com)

> **Maintained by [Petronella Technology Group](https://petronellatech.com)** -- 23+ years in cybersecurity, CMMC Registered Practitioner on staff, 2,500+ companies protected.

---

## Table of Contents

- [What is CMMC 2.0?](#what-is-cmmc-20)
- [CMMC 2.0 Levels Overview](#cmmc-20-levels-overview)
- [Who Needs CMMC Certification?](#who-needs-cmmc-certification)
- [CMMC Timeline and Deadlines](#cmmc-timeline-and-deadlines)
- [Level 1 (Foundational) -- All 17 Practices](#level-1-foundational----all-17-practices)
- [Level 2 (Advanced) -- 110 Practices Overview](#level-2-advanced----110-practices-overview)
- [Self-Assessment vs C3PAO Assessment](#self-assessment-vs-c3pao-assessment)
- [CMMC Scoping Guide](#cmmc-scoping-guide)
- [Common CMMC Pitfalls](#common-cmmc-pitfalls)
- [Repository Contents](#repository-contents)
- [How to Use This Toolkit](#how-to-use-this-toolkit)
- [About Petronella Technology Group](#about-petronella-technology-group)

---

## What is CMMC 2.0?

The **Cybersecurity Maturity Model Certification (CMMC) 2.0** is a Department of Defense (DoD) framework that requires defense contractors to implement cybersecurity practices to protect **Federal Contract Information (FCI)** and **Controlled Unclassified Information (CUI)**. CMMC 2.0 was published as a final rule (32 CFR Part 170) in October 2024 and is being phased into DoD contracts.

### Key Definitions

| Term | Definition |
|------|-----------|
| **FCI** | Federal Contract Information -- Information provided by or generated for the government under a contract that is not intended for public release |
| **CUI** | Controlled Unclassified Information -- Information that requires safeguarding or dissemination controls per law, regulation, or government-wide policy (e.g., technical drawings, test data, export-controlled information) |
| **CCA** | CMMC Certified Assessor -- Individual authorized to conduct CMMC assessments |
| **C3PAO** | CMMC Third-Party Assessment Organization -- Organization authorized to conduct Level 2 certification assessments |
| **OSC** | Organization Seeking Certification -- The defense contractor pursuing CMMC certification |
| **SPRS** | Supplier Performance Risk System -- DoD system where self-assessment scores are recorded |

### CMMC vs. NIST 800-171

CMMC Level 2 is directly mapped to **NIST SP 800-171 Rev 2** (110 security requirements). While NIST 800-171 has been a contractual requirement since 2017 via DFARS 252.204-7012, CMMC adds **third-party verification** -- organizations can no longer simply self-attest to compliance. CMMC ensures that contractors have actually implemented the required controls, not just documented them.

---

## CMMC 2.0 Levels Overview

CMMC 2.0 streamlined the original CMMC 1.0 model from five levels to three:

| Level | Name | Practices | Based On | Assessment Type | Who Needs It |
|-------|------|-----------|----------|----------------|-------------|
| **Level 1** | Foundational | 17 practices | FAR 52.204-21 (Basic Safeguarding) | Annual self-assessment | Contractors handling FCI only |
| **Level 2** | Advanced | 110 practices | NIST SP 800-171 Rev 2 | Self-assessment OR C3PAO assessment (depending on contract) | Contractors handling CUI |
| **Level 3** | Expert | 110+ practices | NIST SP 800-171 Rev 2 + select NIST SP 800-172 | Government-led assessment (DIBCAC) | Contractors handling the most sensitive CUI / highest-priority programs |

### Key Changes from CMMC 1.0 to 2.0

- Reduced from 5 levels to 3 levels
- Eliminated CMMC-unique practices (now fully aligned with NIST standards)
- Introduced self-assessment option for some Level 2 contracts
- Added Plans of Action and Milestones (POA&Ms) with time-limited conditional certification
- Eliminated maturity processes (the "maturity" aspect from CMMC 1.0)

---

## Who Needs CMMC Certification?

**Every organization in the Defense Industrial Base (DIB)** that processes, stores, or transmits FCI or CUI will eventually need CMMC certification. This includes:

- **Prime contractors** with DoD contracts
- **Subcontractors** at any tier who handle FCI or CUI
- **IT service providers and MSPs** supporting defense contractors
- **Cloud service providers** hosting CUI for defense contractors
- **Manufacturers** producing components for DoD programs
- **Research institutions** performing DoD-funded research
- **Consultants and professional services firms** with access to CUI

### How to Determine Your Required Level

1. **Check your contracts** -- Look for DFARS 252.204-7012, 7019, 7020, and 7021 clauses
2. **Identify your data** -- Do you handle FCI only (Level 1) or CUI (Level 2+)?
3. **Check solicitations** -- New contracts will specify the required CMMC level
4. **Review the CMMC Assessment Scope** -- Your contract will specify self-assessment vs. C3PAO assessment for Level 2

> **Not sure?** Most defense contractors handling CUI will need **CMMC Level 2** with a C3PAO assessment.

---

## CMMC Timeline and Deadlines

CMMC 2.0 is being phased into DoD contracts over a four-phase rollout:

| Phase | Timeframe | What Happens |
|-------|-----------|-------------|
| **Phase 1** | Starts with rule effective date (late 2024/early 2025) | Level 1 self-assessment and Level 2 self-assessment may appear in contracts |
| **Phase 2** | Phase 1 + 1 year | Level 2 C3PAO assessments may appear in contracts |
| **Phase 3** | Phase 2 + 1 year | Level 3 assessments may appear in contracts |
| **Phase 4** | Phase 3 + 1 year | Full implementation -- CMMC required in all applicable contracts |

### Critical Action Items

- **Now:** Begin self-assessment against NIST 800-171 and document your SPRS score
- **Now:** Identify your CUI boundary and create a System Security Plan (SSP)
- **Now:** Address gaps and create Plans of Action and Milestones (POA&Ms)
- **Before contract award:** Achieve required CMMC level certification
- **Ongoing:** Maintain certification through continuous monitoring and annual affirmations

---

## Level 1 (Foundational) -- All 17 Practices

Level 1 requires implementation of 17 basic cybersecurity practices derived from **FAR 52.204-21**. These are fundamental security hygiene practices that every organization should have in place.

### Access Control (AC)

| # | Practice ID | Requirement |
|---|------------|-------------|
| 1 | **AC.L1-b.1.i** | Limit information system access to authorized users, processes acting on behalf of authorized users, or devices (including other information systems) |
| 2 | **AC.L1-b.1.ii** | Limit information system access to the types of transactions and functions that authorized users are permitted to execute |
| 3 | **AC.L1-b.1.iii** | Verify and control/limit connections to and use of external information systems |
| 4 | **AC.L1-b.1.iv** | Control information posted or processed on publicly accessible information systems |

### Identification and Authentication (IA)

| # | Practice ID | Requirement |
|---|------------|-------------|
| 5 | **IA.L1-b.1.v** | Identify information system users, processes acting on behalf of users, or devices |
| 6 | **IA.L1-b.1.vi** | Authenticate (or verify) the identities of those users, processes, or devices, as a prerequisite to allowing access to organizational information systems |

### Media Protection (MP)

| # | Practice ID | Requirement |
|---|------------|-------------|
| 7 | **MP.L1-b.1.vii** | Sanitize or destroy information system media containing Federal Contract Information before disposal or release for reuse |

### Physical Protection (PE)

| # | Practice ID | Requirement |
|---|------------|-------------|
| 8 | **PE.L1-b.1.viii** | Limit physical access to organizational information systems, equipment, and the respective operating environments to authorized individuals |
| 9 | **PE.L1-b.1.ix** | Escort visitors and monitor visitor activity; maintain audit logs of physical access |
| 10 | **PE.L1-b.1.x** | Maintain audit logs of physical access |
| 11 | **PE.L1-b.1.xi** | Control and manage physical access devices |

### System and Communications Protection (SC)

| # | Practice ID | Requirement |
|---|------------|-------------|
| 12 | **SC.L1-b.1.xii** | Monitor, control, and protect organizational communications at the external boundaries of the information systems and at key internal boundaries |
| 13 | **SC.L1-b.1.xiii** | Implement subnetworks for publicly accessible system components that are physically or logically separated from internal networks |

### System and Information Integrity (SI)

| # | Practice ID | Requirement |
|---|------------|-------------|
| 14 | **SI.L1-b.1.xiv** | Identify, report, and correct information and information system flaws in a timely manner |
| 15 | **SI.L1-b.1.xv** | Provide protection from malicious code at appropriate locations within organizational information systems |
| 16 | **SI.L1-b.1.xvi** | Update malicious code protection mechanisms when new releases are available |
| 17 | **SI.L1-b.1.xvii** | Perform periodic scans of the information system and real-time scans of files from external sources as files are downloaded, opened, or executed |

> **Full checklist with implementation guidance:** [CMMC Level 1 Checklist](checklists/cmmc-level1-checklist.md)

---

## Level 2 (Advanced) -- 110 Practices Overview

Level 2 implements all 110 security requirements from **NIST SP 800-171 Rev 2**, organized into 14 domains:

| Domain | ID | Number of Practices | Description |
|--------|-----|-------------------|-------------|
| Access Control | AC | 22 | Manage who can access CUI and what they can do |
| Awareness and Training | AT | 3 | Ensure personnel understand security responsibilities |
| Audit and Accountability | AU | 9 | Track and review system activity |
| Configuration Management | CM | 9 | Maintain secure system configurations |
| Identification and Authentication | IA | 11 | Verify user and device identities |
| Incident Response | IR | 3 | Detect, report, and respond to incidents |
| Maintenance | MA | 6 | Maintain systems securely |
| Media Protection | MP | 9 | Protect CUI on digital and physical media |
| Personnel Security | PS | 2 | Screen personnel and protect CUI during personnel actions |
| Physical Protection | PE | 6 | Protect physical facilities and devices |
| Risk Assessment | RA | 3 | Identify and manage risk |
| Security Assessment | CA | 4 | Assess and monitor security effectiveness |
| System and Communications Protection | SC | 16 | Protect communications and system boundaries |
| System and Information Integrity | SI | 7 | Detect and correct system flaws |
| **Total** | | **110** | |

### NIST 800-171 to CMMC Mapping

Every CMMC Level 2 practice maps directly to a NIST 800-171 Rev 2 requirement. For example:

- CMMC **AC.L2-3.1.1** = NIST 800-171 **3.1.1** (Limit system access to authorized users)
- CMMC **IA.L2-3.5.3** = NIST 800-171 **3.5.3** (Use multifactor authentication)
- CMMC **SC.L2-3.13.11** = NIST 800-171 **3.13.11** (Employ FIPS-validated cryptography)

> **Full checklist:** [CMMC Level 2 Checklist](checklists/cmmc-level2-checklist.md)

---

## Self-Assessment vs C3PAO Assessment

CMMC 2.0 offers two paths to Level 2 certification, depending on the sensitivity of the CUI in the contract:

### Self-Assessment (Level 2)

| Aspect | Details |
|--------|---------|
| **When required** | Contracts involving CUI that is NOT associated with critical national security programs |
| **Who performs it** | The Organization Seeking Certification (OSC) performs its own assessment |
| **Score submission** | Results entered into SPRS (Supplier Performance Risk System) |
| **Affirmation** | Senior official must affirm accuracy of results in SPRS annually |
| **POA&Ms allowed** | Yes, with time-limited conditional certification (180 days to close) |
| **Cost** | Internal resources only -- no assessment fees |

### C3PAO Assessment (Level 2)

| Aspect | Details |
|--------|---------|
| **When required** | Contracts involving CUI associated with critical national security programs (identified in solicitation) |
| **Who performs it** | A CMMC Third-Party Assessment Organization (C3PAO) accredited by The Cyber AB |
| **Certification** | Certificate of CMMC Status issued upon successful assessment |
| **Validity** | 3 years, with annual affirmation |
| **POA&Ms allowed** | Yes, with conditional certification status (180 days to close) |
| **Cost** | Varies -- typically $25,000-$150,000+ depending on scope and complexity |

### Which Do You Need?

1. Check the solicitation or contract for the specific CMMC requirement
2. If it says "CMMC Level 2 (Self)" -- self-assessment is sufficient
3. If it says "CMMC Level 2 (C3PAO)" -- you need a third-party assessment
4. When in doubt, prepare for C3PAO assessment (it is the more rigorous path, and you will be ready for either)

---

## CMMC Scoping Guide

Proper scoping is critical to a successful CMMC assessment. You need to define your **CMMC Assessment Scope** -- the boundary within which CUI is processed, stored, or transmitted.

### Asset Categories

CMMC uses the following asset categories for scoping:

| Category | Description | In Scope? |
|----------|-------------|-----------|
| **CUI Assets** | Assets that process, store, or transmit CUI | Yes -- fully assessed |
| **Security Protection Assets** | Assets that provide security functions for the CMMC Assessment Scope (firewalls, SIEM, AD, etc.) | Yes -- fully assessed |
| **Contractor Risk Managed Assets** | Assets that can but are not intended to process CUI (e.g., corporate laptops that could access CUI) | Yes -- assessed for risk management |
| **Specialized Assets** | IoT, OT, government-furnished equipment, test equipment | Yes -- assessed using specialized criteria |
| **Out-of-Scope Assets** | Assets completely isolated from CUI processing | No |

### Scoping Best Practices

1. **Minimize your CUI boundary** -- The smaller your scope, the fewer controls you need to implement and assess
2. **Network segmentation** -- Use VLANs, firewalls, and access controls to isolate CUI processing environments
3. **Dedicated CUI enclaves** -- Consider a separate network/enclave specifically for CUI work
4. **Cloud solutions** -- FedRAMP Moderate (or equivalent) cloud services can handle CUI and simplify your scope
5. **Document everything** -- Your SSP must clearly define the assessment scope and all asset categories

---

## Common CMMC Pitfalls

Based on our experience helping hundreds of defense contractors, these are the most common mistakes:

1. **Underestimating scope** -- CUI flows through more systems than you think. Map data flows thoroughly.
2. **Ignoring subcontractors** -- Your subs need their own CMMC certification if they handle CUI.
3. **Confusing NIST 800-171 compliance with CMMC certification** -- CMMC requires verified implementation, not just documented policies.
4. **Waiting too long** -- Achieving compliance can take 6-18 months. Start now.
5. **Using non-compliant cloud services** -- Email, file sharing, and cloud storage for CUI must meet FedRAMP Moderate equivalency.
6. **Weak POA&Ms** -- POA&Ms must have specific milestones, resources, and completion dates. Vague plans will not pass assessment.
7. **Missing the annual affirmation** -- Both self-assessment and C3PAO certifications require annual affirmation in SPRS.
8. **Incomplete SSP** -- The System Security Plan must describe how every control is implemented in your specific environment.
9. **No evidence** -- Assessors need artifacts (screenshots, configs, policies, logs). Claims without evidence are insufficient.
10. **Trying to do it alone** -- CMMC is complex. Organizations that attempt compliance without experienced guidance frequently fail their first assessment.

---

## Repository Contents

### Checklists

| File | Description |
|------|-------------|
| [cmmc-level1-checklist.md](checklists/cmmc-level1-checklist.md) | All 17 Level 1 practices with implementation guidance |
| [cmmc-level2-checklist.md](checklists/cmmc-level2-checklist.md) | All 110 Level 2 practices organized by domain |
| [cmmc-gap-analysis.md](checklists/cmmc-gap-analysis.md) | Gap analysis template for identifying compliance gaps |

### Templates

| File | Description |
|------|-------------|
| [ssp-outline.md](templates/ssp-outline.md) | System Security Plan outline template |
| [poam-template.md](templates/poam-template.md) | Plan of Action and Milestones template |
| [cmmc-readiness-assessment.md](templates/cmmc-readiness-assessment.md) | Readiness assessment questionnaire |

### Scripts

| File | Description |
|------|-------------|
| [cmmc-l1-self-check.sh](scripts/cmmc-l1-self-check.sh) | Shell script that checks basic Level 1 controls (password policy, encryption, antivirus, firewall, patching) |

---

## How to Use This Toolkit

### For Defense Contractors

1. **Determine your required level** -- Review your contracts and solicitations
2. **Start with the appropriate checklist** -- [Level 1](checklists/cmmc-level1-checklist.md) or [Level 2](checklists/cmmc-level2-checklist.md)
3. **Conduct a gap analysis** -- Use [cmmc-gap-analysis.md](checklists/cmmc-gap-analysis.md) to identify where you fall short
4. **Create your SSP** -- Use [ssp-outline.md](templates/ssp-outline.md) as your starting framework
5. **Document your POA&Ms** -- Track remediation with [poam-template.md](templates/poam-template.md)
6. **Run the self-check script** -- Execute [cmmc-l1-self-check.sh](scripts/cmmc-l1-self-check.sh) on your systems
7. **Assess readiness** -- Complete the [readiness assessment](templates/cmmc-readiness-assessment.md)

### For IT Service Providers / MSPs

1. Use these checklists to evaluate your DIB clients' compliance posture
2. Reference the Level 2 checklist when building CUI enclaves
3. Use the SSP outline to create documentation for clients
4. Run the self-check script during quarterly reviews

### For Compliance Officers

1. Use the gap analysis to benchmark your current NIST 800-171 implementation
2. Create POA&Ms for identified gaps with realistic timelines
3. Use the readiness assessment before scheduling your C3PAO assessment
4. Share Level 1 checklists with business units for quick self-evaluation

---

## About Petronella Technology Group

**[Petronella Technology Group (PTG)](https://petronellatech.com)** has been protecting businesses for over 23 years, with deep expertise in CMMC compliance, NIST 800-171 implementation, and defense contractor cybersecurity. We have protected over 2,500 companies and have a CMMC Registered Practitioner on staff.

### Our CMMC Services

- **CMMC Readiness Assessments** -- Evaluate your current posture against CMMC Level 1, 2, or 3 requirements
- **Gap Analysis and Remediation** -- Identify gaps and implement corrective actions with prioritized roadmaps
- **System Security Plan (SSP) Development** -- Create comprehensive SSPs that document your security controls
- **CUI Enclave Design** -- Architect secure environments for processing, storing, and transmitting CUI
- **POA&M Management** -- Track and close compliance gaps within required timelines
- **C3PAO Assessment Preparation** -- Get assessment-ready with mock assessments and evidence preparation
- **Managed CMMC Compliance** -- Ongoing compliance monitoring, annual affirmations, and continuous improvement
- **ComplianceArmor Platform** -- Our proprietary compliance documentation and tracking platform

### Author

**Craig Petronella** is a 15x published author, CMMC Registered Practitioner, and founder of Petronella Technology Group. With 30+ years of experience in cybersecurity and compliance, Craig has guided hundreds of defense contractors through the CMMC certification process.

**Books by Craig Petronella:**
- [Browse all titles on Amazon](https://www.amazon.com/stores/author/B00PWED8E4?tag=petronella-20)

**Listen to the Encrypted Ambition Podcast:**
- [Apple Podcasts](https://podcasts.apple.com/us/podcast/id1535193769)

---

## Get Help with CMMC Compliance

CMMC compliance is complex and the consequences of non-compliance are severe -- you could lose your DoD contracts. If you need expert guidance:

- **Free Consultation:** [petronellatech.com/contact/](https://petronellatech.com/contact/)
- **Website:** [petronellatech.com](https://petronellatech.com)
- **Phone:** 919-348-4912
- **CMMC Services:** [petronellatech.com/compliance/cmmc/](https://petronellatech.com/compliance/cmmc/)

---

## Contributing

We welcome contributions from the cybersecurity and defense compliance community. Please submit a pull request or open an issue if you have suggestions for improving this toolkit.

## Disclaimer

This toolkit is provided for informational and educational purposes only. It does not constitute legal or compliance advice. CMMC requirements are complex and may vary based on your specific contracts and circumstances. Consult with a qualified CMMC Registered Practitioner or assessor for advice specific to your organization.

## License

This project is licensed under the MIT License -- see the [LICENSE](LICENSE) file for details.

---

**Maintained by [Petronella Technology Group](https://petronellatech.com) -- 23+ years in cybersecurity, 2,500+ companies protected.**

**Author: Craig Petronella, 15x published author and CMMC Registered Practitioner**
