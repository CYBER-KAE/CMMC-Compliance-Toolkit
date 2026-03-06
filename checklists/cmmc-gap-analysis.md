# CMMC Gap Analysis Template | By Petronella Technology Group

Use this template to identify gaps between your current security posture and CMMC requirements. Complete one row for each practice that is NOT MET or PARTIALLY MET.

---

## Organization Information

| Field | Details |
|-------|---------|
| **Organization Name** | |
| **Target CMMC Level** | Level 1 / Level 2 / Level 3 |
| **Analysis Date** | |
| **Performed By** | |
| **Current SPRS Score** | |
| **Target SPRS Score** | 110 (full compliance) |

---

## Gap Analysis Matrix

For each practice that is not fully implemented, document the gap and remediation plan.

### Priority Key
- **P1 (Critical)** -- 5-point weighted deductions in SPRS scoring; must remediate first
- **P2 (High)** -- 3-point weighted deductions; address within 90 days
- **P3 (Medium)** -- 1-point weighted deductions; address within 180 days

---

| Practice ID | NIST Ref | Requirement Summary | Current State | Gap Description | Remediation Action | Priority | Owner | Target Date | Est. Cost | Status |
|------------|----------|-------------------|--------------|----------------|-------------------|----------|-------|-------------|-----------|--------|
| | | | Not Met / Partial | | | P1/P2/P3 | | | | Not Started |
| | | | | | | | | | | |
| | | | | | | | | | | |
| | | | | | | | | | | |
| | | | | | | | | | | |
| | | | | | | | | | | |
| | | | | | | | | | | |
| | | | | | | | | | | |
| | | | | | | | | | | |
| | | | | | | | | | | |

---

## Common Gaps and Recommended Solutions

| Gap Area | Common Finding | Recommended Solution | Typical Cost Range |
|----------|---------------|---------------------|-------------------|
| Multi-Factor Authentication (IA.L2-3.5.3) | MFA not implemented or only on some systems | Deploy MFA across all accounts (Microsoft Entra ID, Duo, etc.) | $3-10/user/month |
| FIPS-Validated Encryption (SC.L2-3.13.11) | Using non-FIPS encryption or no encryption | Deploy BitLocker (FIPS mode), TLS 1.2+, FIPS-validated VPN | $0-5K |
| Audit Logging (AU.L2-3.3.1) | No centralized logging or SIEM | Deploy SIEM solution (Sentinel, Splunk, etc.) | $5-50K/year |
| CUI at Rest (SC.L2-3.13.16) | CUI not encrypted at rest | Enable BitLocker, database encryption, cloud encryption | $0-10K |
| Vulnerability Scanning (RA.L2-3.11.2) | No periodic vulnerability scanning | Deploy scanning tool (Nessus, Qualys, etc.) | $3-15K/year |
| Security Training (AT.L2-3.2.1) | No formal security awareness program | Implement training platform (KnowBe4, etc.) | $10-25/user/year |
| Incident Response (IR.L2-3.6.1) | No documented incident response plan | Develop IRP, train team, conduct tabletop exercise | $5-15K |
| System Security Plan (CA.L2-3.12.4) | No SSP or SSP is incomplete | Develop comprehensive SSP documenting all 110 controls | $10-30K |
| Configuration Management (CM.L2-3.4.1) | No baseline configurations documented | Implement CIS Benchmarks, document baselines, deploy GPO | $5-15K |
| Media Protection (MP.L2-3.8.1) | No controls on removable media | Deploy USB device control policies via endpoint management | $0-5K |

---

## Gap Summary

| Priority | Count | SPRS Point Impact | Est. Total Remediation Cost |
|----------|-------|-------------------|---------------------------|
| P1 (Critical) | | | |
| P2 (High) | | | |
| P3 (Medium) | | | |
| **Total Gaps** | | | |

**Current SPRS Score:** _____

**Projected Score After Remediation:** 110

**Estimated Time to Full Compliance:** _____ months

**Estimated Total Budget:** $_____

---

## Approvals

| Role | Name | Signature | Date |
|------|------|-----------|------|
| Analysis Lead | | | |
| IT Director | | | |
| Senior Management | | | |

---

**Need help with your CMMC gap analysis?** [Contact Petronella Technology Group](https://petronellatech.com/contact/) -- CMMC Registered Practitioner on staff.
