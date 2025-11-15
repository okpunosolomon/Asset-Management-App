# Asset Management App – Streamlining Organisational Asset Lifecycle with Microsoft Power Platform

## 1. Executive Summary
SOL Ltd, a mid-sized professional services organisation, faced recurring challenges managing hardware assets — delayed approvals, manual tracking, and incomplete audit trails.  
As part of a digital transformation initiative, a **Model-Driven Power Apps solution** was designed and deployed to automate the **end-to-end asset lifecycle** — from request initiation to allocation, return, and audit visibility.

The project delivers measurable efficiency gains:
- **92 % faster approval turnaround** through automated workflows.  
- **80 % reduction in IT support tickets** related to asset allocation.  
- **75 % lower administrative costs** via lifecycle automation and governance visibility.  

---

## 2. Business Problem
Before implementation, SOL Ltd managed assets via spreadsheets and emails.  
This led to:
- Poor accountability for asset ownership and status.  
- Long approval cycles involving multiple departments.  
- Lack of audit history for compliance and finance reporting.  
- Limited visibility into asset utilisation and return trends.  

The new Power Platform solution replaces these manual steps with a secure, centralised, and auditable digital process.

---

## 3. Solution Overview
The **Asset Management App** is a Model-Driven Power App built on **Microsoft Dataverse**, integrated with **Power Automate** for workflow automation and **Power BI (future integration)** for real-time reporting.

### Core Capabilities
- Centralised asset inventory and ownership tracking.  
- Role-based access for requesters, managers, and IT admins.  
- Automated approval and policy enforcement flows.  
- Full audit trail for every allocation and return.  
- Embedded business rules to prevent policy violations.  

---

## 4. Solution Architecture

![Solution Overview](Solution%20Visuals/Flowchart%20Assestsmanagement%20App.png)

### Key Components
| Layer | Technology | Description |
|-------|-------------|-------------|
| **App Layer** | Model-Driven Power App | User interface for employees, managers, and IT admins. |
| **Data Layer** | Dataverse | Tables for Assets, Requests, Allocations, and Returns. |
| **Automation Layer** | Power Automate | Approval flows, notifications, and policy enforcement. |
| **Governance Layer** | Security Roles | Restrict CRUD access by business unit and job role. |
| **Reporting Layer** | Power BI (Planned) | Future integration for KPI tracking and audit reporting. |

---

## 5. App Walkthrough

### Asset Allocation Lifecycle
![Main Form with Process Flow](App%20Played%20Visuals/Asset%20Allocations%20Main%20Form%20With%20Completed%20Business%20Process%20Flow.png)

- Users submit new requests through the **Asset Request Form**.  
- Managers receive automated approval notifications via Teams and email.  
- Once approved, IT allocates the asset and logs details in Dataverse.  
- Upon return, the asset status updates to *Available* automatically.

---

### Key App Views
![Active Assets](App%20Played%20Visuals/Active%20Assets%20View.png)  
![Active Allocations](App%20Played%20Visuals/Active%20Asset%20Allocations%20View.png)  
![Dashboard](App%20Played%20Visuals/Asset%20Management%20Dashboard.png)

These provide real-time visibility of asset status, pending approvals, and allocation history.

---

## 6. Cloud Flow Automation

### Policy-Based Approval Flow
![Approval Flow Diagram](Cloud%20Flow%20Approval%20Visuals/Asset%20Allocation%20Outside%20the%20Policy%20Approval%20Request%20Cloud%20Flow.png)

**Logic Summary:**
1. Requests exceeding policy limits trigger a special approval path.  
2. Standard requests auto-route to the line manager for approval.  
3. Notifications are sent via Outlook and Microsoft Teams.  
4. Approvals automatically update asset and request records in Dataverse.

### Flow Execution
![Flow Execution](Cloud%20Flow%20Approval%20Visuals/Asset%20Allocation%20Outside%20the%20Policy%20Approval%20Flow%20Request%20in%20Power%20Automate.png)  
![Approval Outcome](Cloud%20Flow%20Approval%20Visuals/Asset%20Allocation%20Outside%20the%20PolicyRequest%20Approved.png)

---

## 7. Governance & Security

![Security Role Configuration](Solution%20Visuals/App%20Security%20Role.png)

The solution enforces **least-privilege access**:
- **Employees:** Create and view personal requests.  
- **Managers:** Approve or reject asset allocations.  
- **IT Admins:** Manage asset lifecycle and inventory.  

All activities are captured in Dataverse audit logs, ensuring compliance with SOL Ltd’s IT governance policy.

---

## 8. Business Impact

| Metric | Before | After Implementation | Improvement |
|---------|---------|-----------------------|-------------|
| Average approval time | 5 days | < 1 day | 92 % faster |
| IT support tickets | High | Minimal | −80 % |
| Administrative hours/month | 40 h | 10 h | −75 % |
| Policy breaches | Common | Rare | Significantly reduced |

**Key Outcomes:**
- Seamless collaboration between departments.  
- Real-time data visibility and audit readiness.  
- Scalable foundation for future automation and analytics.  

---

## 9. Technical Highlights

- **Dataverse Tables:** Asset, Allocation, Request, Contact, Check Table.  
- **Automation:** Power Automate approval flows (standard and policy-based).  
- **Business Logic:** Custom rules for exception handling.  
- **Deployment:** Managed solution packaged for migration and version control.  
- **Testing:** UAT completed with 100 % pass rate across functional scenarios.  

---

## 10. Future Enhancements

- **Power BI Integration** for visual asset insights.  
- **Barcode/QR Integration** for real-time scanning.  
- **Copilot Integration** for AI-based request handling.  
- **Dataverse Plug-ins** for extended automation.  

---

## 11. Repository Structure
```

📂 App Played Visuals/            → Screenshots from live app
📂 Cloud Flow Approval Visuals/   → Power Automate flow visuals
📂 Solution Visuals/              → Dataverse schema and design visuals
📂 Solution Zip File/             → Managed solution for deployment
📂 Overview PDF Project Presentation/ → Client presentation document
README.md                        → Business & technical overview (this file)

```

---

## 12. Conclusion
The **Asset Management App** demonstrates how Microsoft Power Platform can deliver tangible business value when applied strategically.  
By transforming SOL Ltd’s manual processes into an automated, governed, and transparent system, the organisation achieved faster approvals, improved compliance, and cost efficiency.

This project stands as a blueprint for enterprises seeking to modernise operational workflows through low-code automation and intelligent data management.

---

**Developed by:**  
**Solomon Okpuno**  
Power Platform Consultant | Data & Process Automation Specialist  
[LinkedIn](https://linkedin.com/in/solomon-okpuno-51a907312) · [GitHub](https://github.com/okpunosolomon)
```
