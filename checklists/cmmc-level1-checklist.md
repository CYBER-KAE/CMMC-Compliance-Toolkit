# CMMC Level 1 Checklist -- All 17 Practices | By Petronella Technology Group

A detailed checklist for all 17 CMMC Level 1 (Foundational) practices with implementation guidance, evidence examples, and common pitfalls.

**Assessment Type:** Annual self-assessment (entered into SPRS)
**Based On:** FAR 52.204-21 (Basic Safeguarding of Covered Contractor Information Systems)

---

## How to Use This Checklist

For each practice:
1. Review the requirement and implementation guidance
2. Assess your current implementation status
3. Document your evidence (artifacts that prove implementation)
4. Note any gaps that need remediation

**Status Options:**
- **MET** -- Fully implemented with evidence
- **NOT MET** -- Not implemented or partially implemented
- **N/A** -- Not applicable (document justification)

---

## Access Control (AC) -- 4 Practices

### AC.L1-b.1.i -- Authorized Access Control

**Requirement:** Limit information system access to authorized users, processes acting on behalf of authorized users, or devices (including other information systems).

| Field | Details |
|-------|---------|
| **Status** | [ ] MET / [ ] NOT MET |
| **NIST 800-171 Ref** | 3.1.1 |

**Implementation Guidance:**
- Implement user account management (create, modify, disable, delete accounts)
- Require unique user IDs for all users
- Implement role-based access control (RBAC)
- Disable or remove inactive accounts (90 days of inactivity)
- Disable guest accounts and default accounts
- Require manager approval for new accounts

**Evidence Examples:**
- User account list showing unique IDs
- Account management policy/procedure
- Screenshots of access control configurations
- Active Directory / identity provider settings

**Common Pitfalls:**
- Shared/generic accounts still in use
- Former employee accounts not disabled promptly
- No periodic review of account access

---

### AC.L1-b.1.ii -- Transaction and Function Control

**Requirement:** Limit information system access to the types of transactions and functions that authorized users are permitted to execute.

| Field | Details |
|-------|---------|
| **Status** | [ ] MET / [ ] NOT MET |
| **NIST 800-171 Ref** | 3.1.2 |

**Implementation Guidance:**
- Implement least-privilege access (users only get access they need for their job)
- Use role-based access controls to map permissions to job functions
- Restrict administrative/privileged access to IT administrators only
- Implement separation of duties for sensitive functions
- Restrict access to security-relevant functions (e.g., audit logs, security settings)

**Evidence Examples:**
- Role/permission matrix mapped to job functions
- Screenshots of group policy or RBAC configurations
- Access request and approval process documentation
- Privileged account inventory

**Common Pitfalls:**
- All users have admin rights on their workstations
- No documented role-to-permission mapping
- Broad "everyone" permissions on file shares

---

### AC.L1-b.1.iii -- External System Connections

**Requirement:** Verify and control/limit connections to and use of external information systems.

| Field | Details |
|-------|---------|
| **Status** | [ ] MET / [ ] NOT MET |
| **NIST 800-171 Ref** | 3.1.20 |

**Implementation Guidance:**
- Implement policies governing use of external systems (personal devices, cloud services, partner systems)
- Control connections to external systems through firewalls and network access controls
- Restrict the use of personal devices for FCI/CUI processing
- Require VPN or other secure connections for remote access
- Monitor and log connections to external systems

**Evidence Examples:**
- Acceptable use policy addressing external systems
- Firewall rules restricting outbound connections
- VPN configuration and access logs
- BYOD/personal device policy

**Common Pitfalls:**
- No policy on personal device usage
- Uncontrolled cloud service usage (shadow IT)
- No VPN requirement for remote workers

---

### AC.L1-b.1.iv -- Public Information Control

**Requirement:** Control information posted or processed on publicly accessible information systems.

| Field | Details |
|-------|---------|
| **Status** | [ ] MET / [ ] NOT MET |
| **NIST 800-171 Ref** | 3.1.22 |

**Implementation Guidance:**
- Implement review and approval process before posting content to public-facing systems (website, social media)
- Train authorized individuals on what constitutes FCI
- Ensure FCI is never posted to public-facing systems
- Implement content review processes for public websites
- Restrict who can publish to public-facing systems

**Evidence Examples:**
- Content review and approval procedure
- List of authorized publishers for public systems
- Training records on FCI handling
- Evidence of content review before publication

**Common Pitfalls:**
- No formal review process for website/social media content
- Multiple people with publish access and no oversight
- FCI inadvertently included in public marketing materials

---

## Identification and Authentication (IA) -- 2 Practices

### IA.L1-b.1.v -- Identification

**Requirement:** Identify information system users, processes acting on behalf of users, or devices.

| Field | Details |
|-------|---------|
| **Status** | [ ] MET / [ ] NOT MET |
| **NIST 800-171 Ref** | 3.5.1 |

**Implementation Guidance:**
- Assign unique user IDs to all personnel
- Identify devices through MAC addresses, IP addresses, or certificates
- Identify processes through process IDs, certificates, or service accounts
- Maintain an authoritative source of identity information (Active Directory, identity provider)
- Do not use shared or group accounts

**Evidence Examples:**
- User account inventory showing unique IDs
- Device inventory with identification method
- Active Directory or identity provider configuration
- Policy prohibiting shared accounts

**Common Pitfalls:**
- Shared logins for kiosks or common workstations
- Generic service accounts without proper tracking
- No device identification mechanism

---

### IA.L1-b.1.vi -- Authentication

**Requirement:** Authenticate (or verify) the identities of those users, processes, or devices, as a prerequisite to allowing access to organizational information systems.

| Field | Details |
|-------|---------|
| **Status** | [ ] MET / [ ] NOT MET |
| **NIST 800-171 Ref** | 3.5.2 |

**Implementation Guidance:**
- Require passwords or other authentication factors for all user access
- Implement password complexity requirements (minimum length, complexity, expiration)
- Consider multi-factor authentication (recommended even at Level 1)
- Implement account lockout after failed attempts
- Authenticate devices before granting network access (802.1X, certificates)

**Evidence Examples:**
- Password policy (minimum 8 characters with complexity)
- Group policy/identity provider password settings
- Account lockout policy configuration
- MFA configuration (if implemented)

**Common Pitfalls:**
- No password complexity requirements enforced
- No account lockout policy
- Password policy documented but not technically enforced

---

## Media Protection (MP) -- 1 Practice

### MP.L1-b.1.vii -- Media Sanitization

**Requirement:** Sanitize or destroy information system media containing Federal Contract Information before disposal or release for reuse.

| Field | Details |
|-------|---------|
| **Status** | [ ] MET / [ ] NOT MET |
| **NIST 800-171 Ref** | 3.8.3 |

**Implementation Guidance:**
- Implement media sanitization procedures aligned with NIST SP 800-88
- Use approved sanitization methods: Clear, Purge, or Destroy (based on media type and sensitivity)
- Maintain sanitization records (what was sanitized, when, by whom, method)
- Use certified data destruction vendors for hard drives and other persistent storage
- Address all media types: hard drives, SSDs, USB drives, optical media, mobile devices, printers

**Evidence Examples:**
- Media sanitization policy and procedures
- Sanitization records / certificates of destruction
- Data destruction vendor contract and certificates
- NIST 800-88 compliant procedures documented

**Common Pitfalls:**
- Old hard drives sitting in closets unsanitized
- No record of media disposal
- Printers/copiers with hard drives disposed of without sanitization
- USB drives not tracked or sanitized

---

## Physical Protection (PE) -- 4 Practices

### PE.L1-b.1.viii -- Limit Physical Access

**Requirement:** Limit physical access to organizational information systems, equipment, and the respective operating environments to authorized individuals.

| Field | Details |
|-------|---------|
| **Status** | [ ] MET / [ ] NOT MET |
| **NIST 800-171 Ref** | 3.10.1 |

**Implementation Guidance:**
- Control physical access to facilities with locks, badge readers, or other mechanisms
- Restrict access to server rooms, wiring closets, and areas with FCI systems
- Issue access credentials (keys, badges, codes) only to authorized individuals
- Maintain a list of authorized individuals with physical access
- Implement different access levels based on area sensitivity

**Evidence Examples:**
- Facility access control descriptions (locks, badges)
- Authorized access list for sensitive areas
- Badge/key issuance records
- Server room access controls

**Common Pitfalls:**
- Server room unlocked or using a shared key/code that is never changed
- No distinction between general office access and sensitive area access
- Contractors or visitors with unrestricted access

---

### PE.L1-b.1.ix -- Escort Visitors

**Requirement:** Escort visitors and monitor visitor activity.

| Field | Details |
|-------|---------|
| **Status** | [ ] MET / [ ] NOT MET |
| **NIST 800-171 Ref** | 3.10.3 |

**Implementation Guidance:**
- Implement a visitor management process
- Require all visitors to sign in and be issued visitor badges
- Escort visitors in areas where FCI is processed or stored
- Monitor visitor activity while on premises
- Distinguish visitor badges visually from employee badges

**Evidence Examples:**
- Visitor management policy
- Visitor log (sign-in/sign-out)
- Visitor badge examples (distinguishable from employee badges)
- Escort procedures documentation

**Common Pitfalls:**
- Visitors allowed to roam freely after check-in
- No visitor sign-in/sign-out log
- Visitor badges identical to employee badges

---

### PE.L1-b.1.x -- Maintain Physical Access Logs

**Requirement:** Maintain audit logs of physical access.

| Field | Details |
|-------|---------|
| **Status** | [ ] MET / [ ] NOT MET |
| **NIST 800-171 Ref** | 3.10.4 |

**Implementation Guidance:**
- Maintain logs of physical access to sensitive areas
- Include date, time, individual, and area accessed
- Retain physical access logs per organizational retention policy
- Periodically review physical access logs for anomalies
- Use electronic badge systems or manual sign-in logs

**Evidence Examples:**
- Badge system access reports
- Manual access logs for sensitive areas
- Log review records showing periodic review
- Log retention policy

**Common Pitfalls:**
- No access logs for server room or data center
- Logs exist but are never reviewed
- Logs not retained for adequate period

---

### PE.L1-b.1.xi -- Manage Physical Access Devices

**Requirement:** Control and manage physical access devices.

| Field | Details |
|-------|---------|
| **Status** | [ ] MET / [ ] NOT MET |
| **NIST 800-171 Ref** | 3.10.5 |

**Implementation Guidance:**
- Maintain inventory of all physical access devices (keys, badges, access cards, lock combinations)
- Change combinations and locks when keys are lost or personnel change
- Disable badges for terminated employees immediately
- Periodically audit physical access device inventory
- Control issuance and return of physical access devices

**Evidence Examples:**
- Key/badge inventory list
- Badge deactivation records for terminated employees
- Lock change records
- Physical access device issuance/return log

**Common Pitfalls:**
- Former employees still have active badges
- Lost keys not reported or locks not changed
- No inventory of who has which keys/badges

---

## System and Communications Protection (SC) -- 2 Practices

### SC.L1-b.1.xii -- Boundary Protection

**Requirement:** Monitor, control, and protect organizational communications at the external boundaries of the information systems and at key internal boundaries.

| Field | Details |
|-------|---------|
| **Status** | [ ] MET / [ ] NOT MET |
| **NIST 800-171 Ref** | 3.13.1 |

**Implementation Guidance:**
- Deploy firewalls at network boundaries (internet-facing and between network zones)
- Configure firewalls with deny-by-default / allow-by-exception rules
- Monitor boundary traffic for suspicious activity
- Implement intrusion detection/prevention at boundaries
- Log and review boundary device activity

**Evidence Examples:**
- Firewall configuration showing deny-by-default rules
- Network diagram showing boundary protection points
- Firewall/IDS logs showing monitoring
- Boundary device inventory

**Common Pitfalls:**
- Firewall with overly permissive rules (allow all outbound)
- No monitoring of boundary traffic
- Consumer-grade router instead of enterprise firewall

---

### SC.L1-b.1.xiii -- Public-Facing Subnetwork Separation

**Requirement:** Implement subnetworks for publicly accessible system components that are physically or logically separated from internal networks.

| Field | Details |
|-------|---------|
| **Status** | [ ] MET / [ ] NOT MET |
| **NIST 800-171 Ref** | 3.13.5 |

**Implementation Guidance:**
- Place all public-facing servers (web, email, DNS) in a DMZ
- Physically or logically separate the DMZ from internal networks
- Control traffic between DMZ and internal networks through firewall rules
- Do not allow direct traffic from the internet to internal networks
- If no public-facing systems exist, document that this practice is N/A

**Evidence Examples:**
- Network diagram showing DMZ architecture
- Firewall rules controlling DMZ-to-internal traffic
- Documentation if no public-facing systems exist

**Common Pitfalls:**
- Public-facing web server on the same subnet as internal workstations
- No DMZ implemented
- DMZ firewall rules allow unrestricted traffic to internal network

---

## System and Information Integrity (SI) -- 4 Practices

### SI.L1-b.1.xiv -- Flaw Remediation

**Requirement:** Identify, report, and correct information and information system flaws in a timely manner.

| Field | Details |
|-------|---------|
| **Status** | [ ] MET / [ ] NOT MET |
| **NIST 800-171 Ref** | 3.14.1 |

**Implementation Guidance:**
- Implement a patch management process
- Identify system flaws through vendor advisories, vulnerability scans, and bug reports
- Test patches before deployment (where feasible)
- Deploy critical/high-severity patches within 30 days
- Document patch management activities

**Evidence Examples:**
- Patch management policy
- WSUS/SCCM/Intune patch deployment reports
- Vulnerability scan results showing patch status
- Patch deployment records

**Common Pitfalls:**
- No formal patch management process
- Patches applied inconsistently (some systems skipped)
- Third-party applications not included in patching

---

### SI.L1-b.1.xv -- Malicious Code Protection

**Requirement:** Provide protection from malicious code at appropriate locations within organizational information systems.

| Field | Details |
|-------|---------|
| **Status** | [ ] MET / [ ] NOT MET |
| **NIST 800-171 Ref** | 3.14.2 |

**Implementation Guidance:**
- Deploy antivirus/anti-malware on all endpoints (workstations, servers)
- Deploy email security (anti-spam, anti-phishing, attachment scanning)
- Deploy web filtering to block known malicious sites
- Enable real-time protection and scheduled full-system scans
- Centrally manage endpoint protection for visibility and reporting

**Evidence Examples:**
- Endpoint protection deployment status report (all systems covered)
- Central management console screenshots
- Email security configuration
- Real-time protection enabled confirmation

**Common Pitfalls:**
- Some workstations missing endpoint protection
- Free/consumer antivirus without central management
- Email gateway without attachment/link scanning

---

### SI.L1-b.1.xvi -- Update Malicious Code Protection

**Requirement:** Update malicious code protection mechanisms when new releases are available.

| Field | Details |
|-------|---------|
| **Status** | [ ] MET / [ ] NOT MET |
| **NIST 800-171 Ref** | 3.14.4 |

**Implementation Guidance:**
- Configure automatic signature/definition updates
- Configure automatic engine updates
- Monitor update status across all endpoints
- Address systems that are not receiving updates
- Verify updates are occurring (do not just assume auto-update works)

**Evidence Examples:**
- Endpoint protection console showing current definition dates
- Auto-update configuration settings
- Update status report across all endpoints
- Alert/notification configuration for failed updates

**Common Pitfalls:**
- Auto-update enabled but some systems not receiving updates (network issues, agent issues)
- No monitoring to confirm updates are actually occurring
- Definitions more than 7 days old on some systems

---

### SI.L1-b.1.xvii -- System and File Scanning

**Requirement:** Perform periodic scans of the information system and real-time scans of files from external sources as files are downloaded, opened, or executed.

| Field | Details |
|-------|---------|
| **Status** | [ ] MET / [ ] NOT MET |
| **NIST 800-171 Ref** | 3.14.5 |

**Implementation Guidance:**
- Configure weekly (minimum) full system scans on all endpoints
- Enable real-time/on-access scanning for files from external sources
- Scan removable media (USB drives) upon insertion
- Scan email attachments and web downloads in real-time
- Review and respond to scan findings

**Evidence Examples:**
- Scan schedule configuration
- Scan results/reports showing regular execution
- Real-time scanning configuration
- USB/removable media scanning settings

**Common Pitfalls:**
- Full scans scheduled but not actually running (system off during scan window)
- Real-time scanning disabled due to performance complaints
- Scan results not reviewed or acted upon

---

## Assessment Summary

| Domain | Practices | MET | NOT MET |
|--------|-----------|-----|---------|
| Access Control (AC) | 4 | | |
| Identification and Authentication (IA) | 2 | | |
| Media Protection (MP) | 1 | | |
| Physical Protection (PE) | 4 | | |
| System and Communications Protection (SC) | 2 | | |
| System and Information Integrity (SI) | 4 | | |
| **Total** | **17** | | |

**SPRS Score:** _____ / 110

**Assessment Date:** _______________

**Assessed By:** _______________

**Senior Official Affirmation:** _______________

---

**Need help with CMMC Level 1 compliance?** [Contact Petronella Technology Group](https://petronellatech.com/contact/) -- CMMC Registered Practitioner on staff.
