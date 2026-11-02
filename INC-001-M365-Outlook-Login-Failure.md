# INC-001 — Microsoft 365 Outlook Login Failure

**Project:** Northstar Technologies — GLPI IT Service Desk & Incident Management Lab  
**Environment:** GLPI hosted locally using Docker on macOS  
**Incident type:** Incident  
**Requester:** James Michael (Finance)  
**Initial assignee:** Daniel Okafor (IT Support — L1)  
**Escalated technician:** Chinedu Obi (IT Support — L2)  
**Urgency:** High  
**Impact:** Medium  
**Priority:** High (as displayed in GLPI)  
**Final status:** Closed  
**Recorded date:** 2026-11-02  
**Scope:** Fictional training scenario; no production Microsoft 365 tenant or live Entra ID sign-in logs were accessed.

## 1. Executive summary

A Finance employee reported being unable to sign in to Microsoft 365 Outlook. Restarting the computer and checking internet connectivity did not resolve the reported authentication error. The incident was logged in GLPI, reviewed by Level 1 support, escalated for simulated Level 2 identity troubleshooting, and closed after simulated remediation and requester verification.

The exercise demonstrates service desk ticket handling, ownership, escalation, documented investigation, resolution communication, and incident closure. **The technical findings and successful remediation below are scenario assumptions, not evidence of changes to a real Microsoft 365 account.**

## 2. User-reported issue and business impact

**Ticket title:** `INC-001 | Microsoft 365 Outlook Login Failure`

The requester reported an authentication error when attempting to access Outlook. The issue prevented access to important Finance department emails and disrupted assigned work. The user stated they had restarted the computer and checked connectivity without success.

## 3. Ticket classification

| Field | Recorded value |
|---|---|
| Entity | Northstar Technologies |
| Type | Incident |
| Request source | Helpdesk |
| Urgency | High |
| Impact | Medium |
| Priority | High |
| Requester | James Michael |
| Support groups | IT Support — L1; IT Support — L2 |
| Final status | Closed |
| ITIL category | Not selected in the incident screenshots; category taxonomy was configured later |

## 4. Level 1 triage and investigation

**L1 technician:** Daniel Okafor

The initial investigation plan documented in GLPI was to:

1. Obtain the exact authentication error message.
2. Test Outlook Web Access to distinguish a desktop-only issue from an account-wide issue.
3. Confirm general internet connectivity.
4. Determine whether other employees experienced similar symptoms.
5. Request an authorized review of account status, licensing, and MFA configuration.

**L1 outcome:** The ticket remained under investigation and was escalated for administrator-level identity and authentication checks. No root cause was confirmed during initial triage.

## 5. Escalation to Level 2

**L2 technician:** Chinedu Obi  
**Escalation reason:** Further review of Microsoft Entra ID authentication and Microsoft 365 account configuration was required in the simulation.

The L2 acknowledgement documented a plan to inspect sign-in logs, account status, licensing, Conditional Access and MFA requirements, and whether both Outlook desktop and Outlook Web Access were affected.

## 6. Simulated diagnostic findings

The training scenario recorded the following assumed findings:

- The user account was active in Microsoft Entra ID.
- Microsoft 365 licensing was valid.
- Both Outlook desktop and Outlook Web Access required additional authentication.
- The simulated sign-in investigation pointed to an MFA registration problem.
- The scenario assumed no widespread Microsoft 365 service outage.

**Suspected root cause:** The user's previously registered MFA authentication method was unavailable, preventing successful sign-in.

> Evidence limitation: These findings were entered into GLPI as part of a fictional exercise. They were **not** obtained from live Entra ID sign-in logs, Microsoft 365 admin center, or a production user account.

## 7. Simulated corrective action

The documented remediation workflow was:

1. Verify the requester's identity according to the organization's approved identity-verification process.
2. Have an authorized administrator initiate MFA re-registration using approved procedures.
3. Guide the requester through registering a new authentication method.
4. Test sign-in to Outlook Web Access and Outlook desktop.
5. Confirm mailbox access and email synchronization.

**Scenario outcome:** The simulated MFA re-registration restored Outlook authentication.

## 8. Validation and resolution

The GLPI ticket recorded simulated requester confirmation that:

- Outlook sign-in succeeded.
- The Finance mailbox was accessible.
- A test email was sent and received.
- The original authentication error no longer appeared.

The L2 resolution note attributed the issue to an unavailable MFA authentication method and documented simulated restoration of access. The ticket was moved to **Solved**, then **Closed**.

## 9. Incident lifecycle and workflow

`Reported → New → Assigned to L1 → Investigated → Escalated to L2 → Simulated diagnosis → Simulated remediation → Requester verification → Solved → Closed`

**Observed outcome:** GLPI's ticket list displayed one closed ticket, `INC-001`, with High priority and Daniel Okafor shown in the assigned-technician column. The ticket history also documented Chinedu Obi's L2 investigation and resolution work. This distinction matters: escalation participation does not necessarily replace the original assignee in the final ticket list.

## 10. Skills demonstrated

- GLPI incident creation, classification, assignment, status tracking, and closure
- ITIL-aligned incident management and escalation
- L1 triage planning and documentation
- L2 investigation planning for Microsoft 365 / Entra ID authentication
- MFA incident response workflow and identity verification considerations
- End-user communication and validation of service restoration
- Accurate distinction between simulated findings and live-system evidence

## 11. Screenshots to include

Place redacted screenshots in a `screenshots/` folder and update the filenames below to match your saved images.

| Evidence | Suggested filename | What it shows |
|---|---|---|
| Ticket opened | `screenshots/inc-001-created.png` | Original user report, urgency, impact, and priority |
| L1 investigation | `screenshots/inc-001-l1-investigation.png` | Initial triage plan and investigation notes |
| L2 acknowledgement | `screenshots/inc-001-l2-escalation.png` | Escalation acknowledgement and planned checks |
| Simulated diagnosis | `screenshots/inc-001-l2-findings.png` | MFA-related suspected cause and remediation plan |
| Resolution | `screenshots/inc-001-resolution.png` | Simulated verification and solved status |
| Closure | `screenshots/inc-001-closed.png` | Final Closed status in GLPI ticket list |

> Before publishing, remove passwords, tokens, personal contact details, and any unrelated browser tabs or notifications. Use fictional names only where possible.

## 12. Lessons learned and next improvements

- Separate initial symptoms, diagnostic hypotheses, confirmed findings, and remediation steps.
- Preserve a clear audit trail when incidents transfer between support tiers.
- Verify restored service before resolving and closing a ticket.
- Configure ITIL categories and SLAs early so future incidents can be categorized and measured consistently.
- For a future live lab, collect authorized test-tenant evidence rather than presenting simulated Entra ID findings as actual log analysis.

---

**Portfolio note:** This case study is a controlled service desk simulation built to demonstrate incident management practices. It does not claim production Microsoft 365 administration or real-user account remediation.
