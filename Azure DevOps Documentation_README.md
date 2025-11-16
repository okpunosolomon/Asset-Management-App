# 🧩 Agile Project Delivery Report — Asset Management App (SOL Ltd)

---

## 🧠 Executive Overview

The **Asset Management App** is a Model-Driven Power Apps solution designed to automate the asset lifecycle — from request to approval, allocation, and return — using **Microsoft Dataverse** and **Power Automate**.  
The project followed the **Scrum framework** under an Agile DevOps structure, delivering incremental value across three sprints.

**Objective:**  
Digitise and streamline asset management operations, reduce manual effort, and ensure audit-ready visibility across the organisation.

---

## 🧱 Project Delivery Framework

| Parameter | Details |
|------------|----------|
| **Methodology** | Scrum (3 sprints × 2 weeks) |
| **Toolchain** | Azure DevOps, Power Platform, GitHub |
| **Project Manager / Scrum Master** | Solomon Okpuno |
| **Product Owner** | IT Asset Manager |
| **Delivery Roles** | BA, Developer, QA, End-User Rep |
| **Environments** | DEV / UAT / PROD (Dataverse) |

---

## 🗺️ Agile Kanban Overview

The Azure DevOps board below visualises sprint workflow across **Backlog**, **In Progress**, **Review**, and **Bugs** columns, ensuring traceability of all features, tasks, and epics.
![Azure DevOps Kanban Board](https://github.com/okpunosolomon/Asset-Management-App/blob/main/App%20Played%20Visuals/Azure%20DevOps%20Board.png?raw=true)



---

## 🗂️ Sprint 1 — Foundation & Environment Setup (Weeks 1–2)

**Focus:** Environment setup, Dataverse schema, and workflow mapping.

| Epic | Feature | Description | Acceptance Criteria | Status |
|------|----------|--------------|---------------------|--------|
| **E1** | Environment Setup | Create DEV/PROD Power Platform environments | Environment isolation configured | ✅ |
| **E2** | Dataverse Schema | Define core tables: Assets, Requests, Allocations | Entities created and linked | ✅ |
| **E2** | Security Model | Configure roles: Employee, Manager, IT Admin | Access permissions validated | ✅ |
| **E3** | Workflow Mapping | Design approval flow diagrams | Flow approved by stakeholders | ✅ |

**Key Tasks**
- Configure Dev/Prod environments  
- Build Dataverse tables and relationships  
- Define environment variables  
- Document workflow processes  

**Resolved Bugs**
- *B-01:* Role permissions failed to restrict access → Fixed  
- *B-02:* Asset ID auto-number issue → Corrected formula  

---

## 🚀 Sprint 2 — Core Functionality & Automation (Weeks 3–4)

**Focus:** Develop Power Automate workflows, core business logic, and user interactions.

| Epic | Feature | Description | Acceptance Criteria | Status |
|------|----------|--------------|---------------------|--------|
| **E3** | Asset Request Form | Submit asset requests digitally | All fields validated; auto-save enabled | ✅ |
| **E4** | Approval Workflow | Approve requests via Teams/Outlook | Flow updates Dataverse automatically | ✅ |
| **E4** | Policy Exception Flow | Handle non-standard requests | Escalation triggers correctly | ✅ |
| **E4** | Notifications | Send status updates | Email/Teams alerts at all stages | ✅ |
| **E4** | Allocation Logic | Assign/release assets | Asset availability syncs in Dataverse | ✅ |

**Key Tasks**
- Develop Model-Driven forms for Requests & Allocations  
- Build Power Automate approval and escalation flows  
- Test email/Teams notifications  
- Implement dynamic approval hierarchy  

**Resolved Bugs**
- *B-03:* Duplicate flow triggers → Added concurrency control  
- *B-04:* Wrong notification recipient → Adjusted OData filter  

---

## 📊 Sprint 3 — Testing, Reporting & Go-Live (Weeks 5–6)

**Focus:** Final testing, Power BI dashboarding, UAT, and deployment.

| Epic | Feature | Description | Acceptance Criteria | Status |
|------|----------|--------------|---------------------|--------|
| **E5** | Dashboards | Create real-time KPIs | Loads <5 s; data refresh validated | ✅ |
| **E6** | User Acceptance Testing | Validate end-to-end flow | All test cases passed | ✅ |
| **E7** | User Training | Train employees via Teams | 100% checklist completion | ✅ |
| **E7** | Deployment | Move solution to PROD | Deployed and verified | ✅ |
| **E7** | Support Setup | Establish helpdesk channel | Support mailbox live | ✅ |

**Key Tasks**
- Build Power BI dashboards and Dataverse connectors  
- Conduct UAT walkthroughs  
- Fix post-UAT feedback and retest flows  
- Migrate managed solution to production  
- Train users and establish escalation support  

**Resolved Bugs**
- *B-05:* Dashboard counts not updating → Fixed DAX measure  
- *B-06:* UAT flow delay → Adjusted concurrency threshold  

---

## 🧩 Kanban Metrics Summary

| Category | Count | Notes |
|-----------|--------|-------|
| **Epics** | 7 | Covering setup → deployment |
| **Features** | 15 | Delivered across 3 sprints |
| **User Stories** | 25 | Focused on user-centred outcomes |
| **Tasks** | 30 | Execution-level work items |
| **Bugs** | 6 | All resolved successfully |

---

## 🏁 Deliverables by Sprint

| Sprint | Focus | Key Deliverables | Status |
|---------|--------|------------------|--------|
| Sprint 1 | Environment & Schema | Dataverse setup, roles, workflow maps | ✅ Completed |
| Sprint 2 | Core Automation | Asset request forms, approval flows, notifications | ✅ Completed |
| Sprint 3 | Reporting & Deployment | Dashboards, UAT, go-live, support setup | ✅ Completed |

---

## 💼 Business Value Delivered

- **Approval cycle time reduced:** 48 hrs → 4 hrs  
- **Audit visibility:** Full traceability of asset lifecycle  
- **Error reduction:** 90% fewer manual entry issues  
- **Decision support:** Real-time analytics for managers  
- **Scalability:** Foundation established for governance expansion  

---

## 📁 Repository Reference Map

```

📂 Documentation/
┣ BRD, UAT and USER GUIDE_README.md
┣ README_Agile.md  ← (this document)
📂 Solution Visuals/
┣ Azure DevOps Board.png
┣ Asset Management Architecture.png
📂 App Played Visuals/
┣ Dashboard.png
┣ Contact & Asset Forms
📂 Cloud Flow Approval Visuals/
┣ Power Automate Approval Flow.png
📂 Solution Zip File/
┗ AssetManagementApp_Managed.zip

```

---

## 📞 Contact

**Consultant / Scrum Master:** Solomon Okpuno  
📧 [okpunosolomon20@gmail.com](mailto:okpunosolomon20@gmail.com)  
🔗 [linkedin.com/in/solomon-okpuno-51a907312](https://linkedin.com/in/solomon-okpuno-51a907312)  
💻 [github.com/okpunosolomon](https://github.com/okpunosolomon)

---

> *This Agile report summarises end-to-end project delivery within an Azure DevOps environment, providing traceable evidence of successful Power Platform implementation, testing, and release management.*



