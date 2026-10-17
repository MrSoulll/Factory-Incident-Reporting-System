# Fabrika Ariza Bildirim Sistemi
# 🏭 Factory Incident Reporting System (FIRS)

An enterprise-grade, end-to-end incident management and tracking solution engineered for industrial manufacturing lines. Designed to bridge the operational gap between shop-floor operators and IT infrastructure support, the solution enables field personnel to report hardware malfunctions, network outages, and line stoppages with zero friction, while triggering real-time incident resolution workflows.

---

## 📌 Project Overview

In high-throughput manufacturing environments, unaddressed line stoppages directly translate into operational downtime and financial loss. The **Factory Incident Reporting System** eliminates manual reporting delays and paper-based tracking by introducing a centralized, low-latency digital pipeline:

- Field operators submit incidents directly from mobile devices or industrial floor tablets via **Power Apps**.
- Incident data is logged instantly into centralized **SharePoint Lists** with automatic priority classification based on affected production lines and issue criticality.
- Automated **Power Automate** flows immediately dispatch high-priority email alerts and actionable notifications to on-duty IT support teams to minimize Mean Time to Acknowledge (MTTA).

---

## ⚙️ Key Features

- **Operator-Friendly Interface:** Minimal-click, high-contrast canvas app optimized for touchscreens and mobile devices on the plant floor.
- **Dynamic Severity & Escalation:** Automated priority tagging (Critical, High, Medium, Low) based on line impact and incident category.
- **Automated IT Alerting:** Event-driven Power Automate cloud flows trigger instant high-priority email notifications to the IT support roster.
- **Incident Lifecycle Management:** End-to-end ticket tracking (`Open` ➔ `In Progress` ➔ `Resolved` ➔ `Closed`) with resolution notes, technician assignments, and status updates.
- **Audit Trail & Traceability:** Immutable logging of timestamps, operator info, affected workstations, and resolution history for shift handovers and compliance.

---

## 🛠️ Architecture & Tech Stack

- **Frontend / Client:** Microsoft Power Apps (Canvas App) — Tailored for mobile devices, tablets, and shop-floor terminals.
- **Workflow Automation:** Microsoft Power Automate — Cloud flows handling validation, notification routing, and automated escalation logic.
- **Data Layer:** Microsoft SharePoint Lists — Structured cloud storage for incident records, line inventories, technician assignments, and audit logs.
- **Communication & Alerting:** Office 365 Outlook Connector — Instant dispatch of high-priority incident emails with deep links to tickets.
- **Documentation & Tracking:** Git & GitHub.

---

## 🔄 Workflow

1. **Failure Occurs:** A terminal, peripheral, network switch, or line hardware component malfunctions.
2. **Report Logged:** The operator selects the factory zone, production line, issue category, and description via Power Apps.
3. **Automated Escalation:** Submitting the form creates a SharePoint List entry, triggering a Power Automate flow that generates a unique ticket ID and fires an urgent alert to the IT team.
4. **Resolution:** IT engineers take ownership of the ticket, update remediation steps, and mark it resolved for shift reporting.
   
<img width="760" height="636" alt="Ekran görüntüsü 2026-09-12 191956" src="https://github.com/user-attachments/assets/a8344f9a-afe3-4275-a80a-7939745d385f" />
<img width="1919" height="847" alt="Ekran görüntüsü 2026-09-12 192007" src="https://github.com/user-attachments/assets/f1b7be7c-09be-4966-9c40-2668f258aafd" />

