## Overview

This project demonstrates a real-world Identity and Access Management (IAM) environment 
built using Microsoft Entra ID (Azure AD). It simulates enterprise-level security 
infrastructure across three phases: user provisioning, Zero Trust enforcement, and 
Single Sign-On (SSO) integration.

## What Was Built

### Phase 1 — User & Group Management (RBAC)
- Created 5 user accounts representing cross-functional roles (employees, HR, IT admin)
- Organized users into security groups: Employee, HR, and IT
- Applied Role-Based Access Control (RBAC) following the Principle of Least Privilege
  - IT Admins → Helpdesk Administrator role
  - HR Managers → User Administrator role

### Phase 2 — Zero Trust via Conditional Access Policies
- **Block non-US access** — denies all sign-in attempts from outside the United States
- **MFA for admins** — requires multi-factor authentication for all privileged accounts
- **MFA for risky sign-ins** — challenges anomalous or flagged logins with MFA instead 
  of outright blocking, balancing security with usability

### Phase 3 — SAML-Based Single Sign-On (SSO)
- Registered an enterprise application and configured SAML as the authentication method
- Mapped attributes and claims (email, name) through the SAML token
- Assigned all three security groups to the application for group-based access provisioning

## Skills Demonstrated
- Microsoft Entra ID / Azure Active Directory
- Identity & Access Management (IAM)
- Role-Based Access Control (RBAC)
- Zero Trust Security Architecture
- Conditional Access Policy Design
- SAML 2.0 / Single Sign-On (SSO)
