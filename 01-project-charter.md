# Project Charter
## Loan Origination System (LOS)
### Horizon Community Bank — Texas, USA

---

## Document Information

| Field | Details |
|---|---|
| Document Title | Project Charter — Loan Origination System |
| Version | 1.0 |
| Date | July 2025 |
| Author | Business Analyst |
| Status | Approved |

---

## 1. Project Background

Horizon Community Bank is a regional retail bank headquartered in Austin, Texas, serving approximately 85,000 customers across 12 branches in Texas. The bank offers personal loans, home equity loans, auto loans, and small business loans.

Currently, all personal loan applications are processed manually. Customers visit a branch or call the loan department, a Relationship Manager collects information on paper forms, and the application is passed through multiple departments via email for credit assessment and approval.

This manual process is slow, error-prone, and creates significant compliance risk. The bank's leadership has approved a digital transformation initiative to build an online Loan Origination System to address these issues.

---

## 2. Problem Statement

| # | Problem | Business Impact |
|---|---|---|
| P01 | Loan applications processed manually via paper forms and email | 8–10 working days average processing time |
| P02 | No centralized system — data tracked on individual spreadsheets | High error rate, data inconsistency across departments |
| P03 | Customers have no visibility into application status | High volume of inbound status inquiry calls |
| P04 | Credit assessment done manually without system integration | Inconsistent decisions, compliance risk under ECOA |
| P05 | No audit trail for approval decisions | Regulatory risk under CFPB examination guidelines |

---

## 3. Project Objectives

| # | Objective | Success Metric | Target |
|---|---|---|---|
| OB01 | Reduce loan processing time | Average days from application to decision | From 8–10 days to under 48 hours |
| OB02 | Reduce manual data entry errors | Error rate per 100 applications | Reduce by 70% within 6 months of go-live |
| OB03 | Improve customer experience | Customer satisfaction score (CSAT) | Achieve CSAT score of 4.2 / 5.0 |
| OB04 | Ensure regulatory compliance | CFPB audit findings | Zero findings related to LOS in next examination |
| OB05 | Increase loan application volume | Monthly applications processed | 25% increase within 12 months of go-live |

---

## 4. Project Scope

### In Scope

- Online loan application portal for personal loans (web-based)
- Customer registration and identity verification
- Digital document upload (pay stubs, ID, bank statements)
- Automated FICO score retrieval via credit bureau integration
- Credit assessment rules engine
- Multi-level approval workflow (Loan Officer → Credit Manager → Senior Approver)
- Automated customer notifications via email and SMS
- Loan officer and manager dashboards
- Regulatory compliance controls (ECOA, FCRA, GLBA, CFPB)
- Audit trail for all decisions and actions
- Reporting dashboard for management

### Out of Scope

- Mobile application (Phase 2)
- Home equity loans and auto loans (Phase 2)
- Small business loan origination (separate project)
- Core banking system replacement
- Loan servicing and repayment management
- Third-party broker portal

---

## 5. Project Constraints

| Type | Constraint |
|---|---|
| Budget | $480,000 USD total project budget |
| Timeline | Go-live within 8 months of project kick-off |
| Technology | Must integrate with existing Fiserv core banking platform |
| Regulatory | Must comply with ECOA, FCRA, GLBA, and CFPB guidelines |
| Data | All customer data must be stored within US borders |
| Security | Must meet PCI-DSS standards for financial data handling |

---

## 6. Project Assumptions

| # | Assumption |
|---|---|
| A01 | Fiserv core banking platform has available APIs for customer identity verification |
| A02 | Credit bureau (Experian) has an available API for automated FICO score retrieval |
| A03 | Customers have valid email addresses and US mobile numbers on file |
| A04 | Loan officers and credit managers will receive system training before go-live |
| A05 | Legal team will review and approve all compliance controls before UAT |
| A06 | IT infrastructure can support 300 concurrent users at launch |

---

## 7. Project Risks

| Risk# | Risk Description | Likelihood | Impact | Mitigation |
|---|---|---|---|---|
| R01 | Experian API integration delayed or unavailable | Medium | High | Identify backup credit bureau (TransUnion) in Week 2 |
| R02 | Fiserv core banking API documentation incomplete | Medium | High | IT team to confirm API availability in discovery phase |
| R03 | Regulatory requirements change during project | Low | High | Legal team engaged throughout, not just at end |
| R04 | Loan officer resistance to new system | Medium | Medium | Include loan officers in UAT, conduct change management sessions |
| R05 | Scope creep from business stakeholders | High | Medium | Project Charter and BRD sign-off enforced, formal change request process |
| R06 | Customer adoption of online portal lower than expected | Medium | Medium | Marketing campaign 4 weeks before go-live |

---

## 8. Project Team

| Role | Name | Responsibility |
|---|---|---|
| Project Sponsor | Sarah Mitchell, VP Retail Banking | Executive approval, budget authority |
| Project Manager | David Carr | Timeline, budget, resource management |
| Business Analyst | Chandu | Requirements, documentation, stakeholder engagement |
| IT Lead | Marcus Webb | Technical architecture, development oversight |
| Compliance Officer | Linda Torres | Regulatory review and approval |
| Loan Operations Lead | Jennifer Hayes | Business process knowledge, UAT lead |
| Credit Risk Manager | Robert Kim | Credit assessment rules, approval workflow |

---

## 9. High-Level Timeline

| Phase | Activities | Duration |
|---|---|---|
| Phase 1 — Discovery | Stakeholder engagement, elicitation, requirements gathering | Weeks 1–4 |
| Phase 2 — Analysis | Requirements documentation, BRD, process flows | Weeks 5–8 |
| Phase 3 — Design | FSD, wireframes, UI/UX design, technical architecture | Weeks 9–14 |
| Phase 4 — Build | Development, unit testing | Weeks 15–24 |
| Phase 5 — Testing | SIT, UAT, compliance review | Weeks 25–30 |
| Phase 6 — Go-Live | Training, deployment, hypercare | Weeks 31–32 |

---

## 10. Sign-off

*By signing below, stakeholders confirm they have reviewed and approved this Project Charter. This document authorises the project to proceed to the requirements and analysis phase.*

| Name | Role | Signature | Date |
|---|---|---|---|
| Sarah Mitchell | VP Retail Banking / Sponsor | Approved | July 2025 |
| David Carr | Project Manager | Approved | July 2025 |
| Linda Torres | Compliance Officer | Approved | July 2025 |
| Marcus Webb | IT Lead | Approved | July 2025 |
