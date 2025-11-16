# Asset Management App Documentation (SOL Ltd)

---

## 1. Business Requirements Document (BRD)

![Banner](https://github.com/okpunosolomon/Asset-Management-App/blob/main/Solution%20Visuals/A_banner_image_for_an_Asset_Management_App_display.png?raw=true)

### Project Title

**Asset Management App – Streamlining Organisational Asset Lifecycle with Microsoft Power Platform**

### Prepared By

**Solomon Okpuno**
Business & Power Platform Consultant – SOL Ltd

---

### Executive Summary

SOL Ltd required a unified solution to manage the full lifecycle of organisational assets — from request and approval to allocation and recovery. Manual handling caused inconsistencies, approval delays, and limited audit visibility.

The Model-Driven Power App built on **Microsoft Dataverse** and **Power Automate** delivers:

* Centralised asset tracking
* Automated approvals
* Audit transparency and compliance
* Role-based access and dashboards

![Dashboard Overview](https://github.com/okpunosolomon/Asset-Management-App/blob/main/Solution%20Visuals/ca9c0705-1733-4b80-93f2-64d7a14084d9.png?raw=true)

---

### Business Objectives

| Objective              | Description                         | Expected Outcome     |
| ---------------------- | ----------------------------------- | -------------------- |
| Centralise asset data  | Replace spreadsheets with Dataverse | One unified database |
| Automate approvals     | Power Automate workflows            | 60% faster approvals |
| Improve accountability | Role-based tracking                 | Complete visibility  |
| Enforce compliance     | Policy checks via business rules    | Fewer violations     |
| Generate insights      | Power BI dashboards (Phase 2)       | Real-time metrics    |

---

### Stakeholders

| Role          | Name / Department  | Responsibility                      |
| ------------- | ------------------ | ----------------------------------- |
| Sponsor       | Head of Operations | Approve project direction           |
| Process Owner | IT Asset Manager   | Define workflows and policies       |
| End Users     | All Departments    | Request and track assets            |
| System Admin  | IT Admin           | Manage users and access             |
| Consultant    | Solomon Okpuno     | Deliver design, build, and training |

---

### Current Challenges

![Challenge Illustration](https://github.com/okpunosolomon/Asset-Management-App/blob/main/Solution%20Visuals/b32103d8-ed33-4c52-a678-7b0ab1b3c515.png?raw=true)

* Manual email-based asset requests
* Delayed approvals and lost requests
* No unified visibility or audit logs
* Inconsistent record-keeping

---

### Proposed Solution

![Solution Architecture](https://github.com/okpunosolomon/Asset-Management-App/blob/main/Solution%20Visuals/e7d7f14a-1572-4a9f-bb76-f9da9172e7f2.png?raw=true)

* **Model-Driven App:** Unified user interface for requests and tracking
* **Dataverse:** Backend for storing requests, allocations, and history
* **Power Automate:** Automated notifications and approval flows
* **Role-Based Access:** Enforced data security
* **Power BI (Planned):** Lifecycle insights

---

### High-Level Scope

**In Scope**

* Request, approval, allocation, return
* Policy validation, escalation flows
* Email and Teams notifications

**Out of Scope**

* ERP or procurement integrations (Phase 3)

---

### Success Metrics

![Metrics Dashboard](https://github.com/okpunosolomon/Asset-Management-App/blob/main/Solution%20Visuals/8862f54a-2d01-4edd-b4ae-9421312a8667.png?raw=true)

* 60% reduction in approval delays
* 100% traceability of asset movements
* 90% fewer manual data errors

---

### Risks & Mitigation

| Risk               | Mitigation                      |
| ------------------ | ------------------------------- |
| User resistance    | Conduct end-user workshops      |
| Flow failure       | Add error notifications         |
| Security misconfig | Test permissions before go-live |

---

### Sign-Off

| Role             | Name           | Signature |
| ---------------- | -------------- | --------- |
| Project Sponsor  |                |           |
| IT Asset Manager |                |           |
| Consultant       | Solomon Okpuno | ✅         |

---

## 2. User Acceptance Testing (UAT)

### Purpose

Confirm that the solution meets all business requirements and operates as intended before deployment.

---

### UAT Test Scenarios

| ID      | Scenario             | Steps                           | Expected Result                  | Status |
| ------- | -------------------- | ------------------------------- | -------------------------------- | ------ |
| UAT-001 | Submit asset request | Employee logs in, submits form  | Status set to *Pending Approval* | ✅      |
| UAT-002 | Approve request      | Manager reviews and approves    | Status = *Approved*              | ✅      |
| UAT-003 | Reject request       | Manager rejects                 | Status = *Rejected*              | ✅      |
| UAT-004 | Allocate asset       | IT Admin assigns asset          | Status = *Allocated*             | ✅      |
| UAT-005 | Return asset         | Update allocation to *Returned* | Status = *Available*             | ✅      |
| UAT-006 | Policy exception     | Create out-of-policy request    | Escalation flow triggered        | ✅      |
| UAT-007 | Dashboard view       | Manager opens dashboard         | Metrics display correctly        | ✅      |
| UAT-008 | Role-based access    | Employee login                  | Restricted view confirmed        | ✅      |
| UAT-009 | Notification test    | Submit approval request         | Email/Teams alert sent           | ✅      |

![Flow Overview](https://github.com/okpunosolomon/Asset-Management-App/blob/main/Solution%20Visuals/b7dfa8b6-34bd-4e30-9e75-a8cec889903b.png?raw=true)

---

### Sign-Off Summary

| Role             | Name           | Signature | Date |
| ---------------- | -------------- | --------- | ---- |
| Project Sponsor  |                |           |      |
| IT Asset Manager |                |           |      |
| Consultant       | Solomon Okpuno | ✅         |      |

---

## 3. User Guide / Training Manual

### Application Name

**Asset Management App** – SOL Ltd

![App Interface](https://github.com/okpunosolomon/Asset-Management-App/blob/main/Solution%20Visuals/91de6abd-b09a-4ac6-84e0-857b717a19c5.png?raw=true)

---

### Access

1. Visit [https://make.powerapps.com](https://make.powerapps.com)
2. Launch **Asset Management (Model-Driven App)**
3. Sign in using SOL Ltd Microsoft 365 account

---

### User Roles

| Role     | Permissions                         |
| -------- | ----------------------------------- |
| Employee | Create and view own asset requests  |
| Manager  | Approve/reject requests             |
| IT Admin | Allocate, track, and recover assets |
| Admin    | Manage users, flows, and tables     |

---

### Key Features

#### 1. Create a New Request

* Go to **Asset Requests** → *New*
* Complete asset details and justification
* Click *Submit for Approval*

#### 2. Approvals

* Managers receive approval email/Teams alerts
* Approve/reject within app or via link

#### 3. Allocation

* IT Admin allocates from **Assets Table**
* Allocation appears under **Active Assets**

#### 4. Returns

* Admin updates status to *Returned*
* Dataverse changes asset status to *Available*

#### 5. Outside Policy Requests

* Flow triggers secondary approval for policy violations

#### 6. Dashboards

![Dashboard Example](https://github.com/okpunosolomon/Asset-Management-App/blob/main/Solution%20Visuals/ca9c0705-1733-4b80-93f2-64d7a14084d9.png?raw=true)

* Access visual summary of pending approvals, total assets, and departmental distribution

---

### Notifications

* Power Automate sends alerts for submission, approval, allocation, and returns.

---

### Troubleshooting

| Issue                 | Resolution                           |
| --------------------- | ------------------------------------ |
| App not loading       | Verify license or role access        |
| Missing notifications | Check Outlook junk or Teams activity |
| Data not refreshing   | Sync Dataverse tables                |

---

### Support

**Support Email:** [support@sol-ltd.com](mailto:support@sol-ltd.com)
**Phone:** +44 (0)20 5555 0123
**Consultant Contact:** Solomon Okpuno

---

### Version History

| Version | Date     | Description        | Author         |
| ------- | -------- | ------------------ | -------------- |
| 1.0     | Nov 2025 | Initial Deployment | Solomon Okpuno |
