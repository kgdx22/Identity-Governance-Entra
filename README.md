# Identity Governance-Entra

## Overview

This project demonstrates the implementation of Microsoft Entra Identity Governance to manage user access throughout the identity lifecycle. It builds on automated onboarding by introducing governed access through catalogs, access packages, access reviews, and lifecycle workflows.

The solution enforces least-privilege access by granting users time-bound, reviewed access to resources through entitlement management, while automating onboarding and offboarding actions to reduce manual intervention and security risk.

This governance layer integrates with an automated onboarding workflow to provide a complete joiner–mover–leaver identity lifecycle.

---

## 🧩 1. Group-Based License Assignment
<img width="959" height="505" alt="IAMLAB7" src="https://github.com/user-attachments/assets/727ab816-6367-4fba-983d-455001631661" />

---

Configured Microsoft 365 licenses to be assigned through a governed security group. This ensures that when access is granted via Identity Governance, users automatically receive required licenses without manual intervention.

- Enforces consistency
- Prevents license drift
- Aligns access with governance workflows

## 📁 2. Catalog Creation
<img width="959" height="497" alt="IAMLAB4" src="https://github.com/user-attachments/assets/d9a95292-e2c0-4192-8d22-04d12683e353" />

---

Created a dedicated Identity Governance catalog to logically group onboarding-related resources and establish administrative boundaries.

### Catalog Resource Definition
<img width="959" height="497" alt="IAMLAB13" src="https://github.com/user-attachments/assets/e40457d5-d85c-4efe-82f9-5d59b86c42cd" />

---

Added security groups and governed resources to the catalog, defining the scope of access that can be managed through entitlement workflows.

  - Centralizes entitlement management
  -  Simplifies access package design
  -   Enables scalable governance

## 🎟️ 3. Entitlement Management (Access Package Creation)
<img width="959" height="500" alt="IAMLAB5" src="https://github.com/user-attachments/assets/6224cc0b-03c1-4c1d-90af-21ebf52c1b1b" />

---

Created an access package tied to the onboarding catalog, defining what access users can request and receive.

## ⏱️ 4. Expiration & Access Reviews
<img width="959" height="497" alt="IAMLAB9" src="https://github.com/user-attachments/assets/586edc87-db00-419d-820d-8d1d6a9b3e77" />

---

Configured:

- 90-day automatic access expiration

- Monthly access reviews with a 14-day review window

  -  Enforces time-bound access
  -  Enables continuous validation
  -  Supports audit and compliance requirements
 
## 🔄 5. Onboarding Lifecycle Workflow Integration
<img width="959" height="499" alt="IAMLAB10" src="https://github.com/user-attachments/assets/22a82413-64a2-46ef-9a4c-359fbb81f278" />

---

Integrated the access package into an onboarding lifecycle workflow. When users enter scope, the workflow automatically initiates an access package request.

### 📨 Automated Onboarding Tasks
<img width="959" height="466" alt="IAMLAB11" src="https://github.com/user-attachments/assets/cf9bc0dc-8189-4688-a732-91b70eb0257c" />

---

Configured tasks to:

- Request governed access via access package

- Send onboarding notifications

  -  Removes manual access assignment
  -  Ensures governance is applied at onboarding
  -  Aligns provisioning with policy

## 🚪 6. Offboarding & Deprovisioning
<img width="959" height="498" alt="IAMLAB12" src="https://github.com/user-attachments/assets/921314d7-26f7-4aff-bcaf-df448e3020bd" />

---

Implemented offboarding workflows to automate access removal and deprovisioning, ensuring users lose access promptly when leaving or changing roles.

- Reduces lingering access risk
- Enforces least privilege
- Completes the joiner–mover–leaver lifecycle

