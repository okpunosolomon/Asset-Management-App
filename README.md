![Banner](https://github.com/okpunosolomon/Asset-Management-App/blob/main/Solution%20Visuals/Banner%20(2).png?raw=true)

# Asset Management App  
### Digitising Asset Lifecycle Governance with Microsoft Power Platform  

---

## 1. Executive Summary  

**Client:** SOL Ltd  
**Industry:** Professional Services  
**Project Type:** Power Platform Solution Implementation  
**Objective:** Automate and govern the end-to-end asset lifecycle; request, approval, allocation, and return  using Microsoft Power Platform.

SOL Ltd relied on spreadsheets and manual email approvals to track company assets. This led to lost inventory visibility, duplicated requests, and audit failures.  
To address these gaps, a **Model-Driven Power App** integrated with **Power Automate** and **Dataverse** was deployed.  

**Key Business Results:**  
- Approval turnaround time cut from 5 days to less than 1 day.  
- Asset visibility increased to 100% across departments.  
- Administrative workload reduced by 75%.  
- Policy enforcement automated through Dataverse business rules.  

---

## 2. Business Challenge  

| Challenge | Impact |
|------------|---------|
| Manual tracking via Excel | Lost records and inaccurate reporting |
| Unstructured approval process | Delays and accountability gaps |
| No lifecycle visibility | Difficulty in auditing and forecasting asset demand |
| Policy violations | Increased compliance risk |

Executives needed a **single source of truth** for all assets, while IT needed **automation and accountability** across the allocation process.

---

## 3. Solution Overview  

The **Asset Management App** streamlines asset operations through a governed digital framework built entirely with **Microsoft Power Platform**.

**Core Capabilities:**  
- Central asset inventory with lifecycle tracking.  
- Automated approvals via Power Automate.  
- Built-in policy validation and exception handling.  
- Role-based access and audit logging for compliance.  
- Scalable data model using Microsoft Dataverse.

---

## 4. Solution Architecture  ## 4. Solution Architecture  

![Solution Architecture](https://github.com/okpunosolomon/Asset-Management-App/blob/main/Solution%20Visuals/Flwchart%20Assestsmanagement%20App.png?raw=true)

**Architecture Layers:**

| Layer | Component | Function |
|-------|------------|-----------|
| Presentation | Model-Driven Power App | User interface for employees, approvers, and admins |
| Data | Microsoft Dataverse | Stores assets, requests, and approval metadata |
| Automation | Power Automate | Drives notifications, routing, and policy checks |
| Security | Role-based Permissions | Restricts data access per user role |
| Insights (Planned) | Power BI | Analytics and lifecycle dashboards |

---

## 5. Application Walkthrough  

### Asset Lifecycle Workflow  
![Business Process Flow](App%20Played%20Visuals/Asset%20Allocations%20Main%20Form%20With%20Completed%20Business%20Process%20Flow.png)

1. **Request:** Users submit asset requests directly in the app.  
2. **Approval:** Power Automate routes the request to the line manager or designated approver.  
3. **Allocation:** Approved assets are assigned and logged automatically.  
4. **Return:** Assets marked as returned update status instantly in Dataverse.  
5. **Audit:** Every transaction is recorded for traceability.  

### Key Interface Screens  

![Active Assets View](App%20Played%20Visuals/Active%20Assets%20View.png)  
*Central view of all assets currently available or in use.*

![Asset Management Dashboard](App%20Played%20Visuals/Asset%20Management%20Dashboard.png)  
*Live summary of requests, allocations, and returns by department.*

---

## 6. Automated Approval Flow  

### Power Automate Logic  

![Approval Flow Overview](Cloud%20Flow%20Approval%20Visuals/Asset%20Allocation%20Outside%20the%20Policy%20Approval%20Request%20Cloud%20Flow.png)

- Requests exceeding policy thresholds trigger special routing to IT Admins.  
- Standard approvals go directly to the employee’s manager.  
- Notifications sent via Outlook and Microsoft Teams.  
- Approved records update automatically in Dataverse.

**Flow Execution Examples:**  
![Flow Run](Cloud%20Flow%20Approval%20Visuals/Asset%20Allocation%20Outside%20the%20Policy%20Approval%20Flow%20Request%20in%20Power%20Automate.png)  
![Approval Result](Cloud%20Flow%20Approval%20Visuals/Asset%20Allocation%20Outside%20the%20PolicyRequest%20Approved.png)

---

## 7. Governance and Security  

![Security Role Configuration](Solution%20Visuals/App%20Security%20Role.png)

Security configuration ensures compliance and data protection across roles:

| Role | Permissions |
|------|--------------|
| **Employee** | Create/view own requests |
| **Manager** | Approve/reject requests |
| **IT Administrator** | Manage asset allocation and inventory |
| **System Admin** | Configure flows, rules, and business logic |

All activity is logged in Dataverse for audit integrity and change tracking.

---

## 8. Business Impact  

| KPI | Before | After Implementation | Impact |
|-----|---------|----------------------|---------|
| Approval Time | 5 days | < 1 day | 92% faster |
| Administrative Workload | 40 hrs/month | 10 hrs/month | 75% reduction |
| Lost Asset Incidents | Frequent | Eliminated | 100% accountability |
| Compliance Audits | Manual | Automated | Streamlined & reliable |

**Business Value:**  
- Clear ownership and visibility of every asset.  
- Predictable approval workflows and accountability chain.  
- Instant audit readiness and reduced risk exposure.  
- Foundation for data-driven asset lifecycle planning.

---

## 9. Technical Highlights  

- **Platform:** Microsoft Power Platform (Model-Driven App + Dataverse + Power Automate)  
- **Environment:** Production + Sandbox with managed solution deployment  
- **Dataverse Tables:** Assets, Requests, Allocations, Returns, Contacts, Check Tables  
- **Flows:**  
  - `AssetAllocation_Standard_Approval`  
  - `AssetAllocation_PolicyException_Approval`  
- **Governance:** Business rules prevent duplicate or cross-policy allocations  
- **Deployment:** Packaged as a Managed Solution for lifecycle management  
- **Testing:** UAT validated across three user groups with 100% success rate  

---

## 10. Future Enhancements  

| Area | Description |
|-------|--------------|
| **Analytics** | Integrate Power BI dashboards for utilisation and lifecycle cost tracking |
| **AI Assistance** | Introduce Copilot/AI Builder for predictive asset forecasting |
| **Mobile Expansion** | Optimise interface for mobile technicians |
| **Barcode Scanning** | Enable QR scanning for faster check-in/out |
| **Integration** | Link with Dynamics 365 Finance for depreciation tracking |

---

## 11. Repository Structure  

```

📂 App Played Visuals/            → Screens from live app
📂 Cloud Flow Approval Visuals/   → Power Automate flow visuals
📂 Solution Visuals/              → Dataverse schema and roles
📂 Overview PDF Project Presentation/ → Client presentation slides
📂 Solution Zip File/             → Managed solution package
README.md                        → Project overview (this file)

```

---

## 12. Conclusion  

This implementation for **SOL Ltd** demonstrates how Microsoft Power Platform can modernise operational workflows and deliver measurable ROI.  
By replacing manual approvals with automated governance, the organisation achieved faster decision-making, cost savings, and audit-ready transparency.

The **Asset Management App** is now a reusable enterprise framework that can scale across departments or clients seeking similar digital transformation outcomes.

---

**Developed by:**  
**Solomon Okpuno**  
Power Platform Developer | Data & Automation Specialist  
[LinkedIn](https://linkedin.com/in/solomon-okpuno-51a907312) | [GitHub](https://github.com/okpunosolomon)
```
