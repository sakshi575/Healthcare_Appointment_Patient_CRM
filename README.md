# 🏥 Healthcare Appointment & Patient CRM

> An enterprise-grade, end-to-end Salesforce CRM built for seamless healthcare practice management—covering patient intake, doctor scheduling, clinical prescriptions, automated billing, and advanced analytics.

[![Salesforce Platform](https://img.shields.io/badge/Platform-Salesforce%20Developer%20Edition-00A1E0?style=flat&logo=salesforce)](https://developer.salesforce.com/)
[![Apex & LWC](https://img.shields.io/badge/Tech-Apex%20%7C%20LWC%20%7C%20Visualforce-blueviolet)](https://developer.salesforce.com/)
[![Status](https://img.shields.io/badge/Status-Completed-success)](https://github.com/sakshi575/Healthcare_Appointment_Patient_CRM)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

---

## 📖 About the Project

Developed as a **Final-Year B.Tech Computer Science and Engineering (Data Science)** project by **Sakshi Singh**, this solution bridges clinical operations and customer relationship management (CRM) on the Salesforce Platform. It replaces legacy manual record-keeping with a secure, automated, and connected healthcare ecosystem.

---

## ✨ Key Features

*   **Unified Data Model:** Centralized management of Patients, Doctors, and Appointments in a single relational structure.
*   **Clinical & Financial Tracking:** Linked prescriptions and automated billing/payment status tracking per appointment.
*   **Advanced Flow Automation:**
    *   *Screen Flow:* Guided data entry wizards for intuitive patient onboarding.
    *   *Record-Triggered Flow:* Real-time automated updates and notifications.
    *   *Scheduled Flow:* Automated background tasks and appointment follow-ups.
*   **Governance & Approvals:** Custom Approval Process for clinical sign-offs and administrative requests.
*   **Custom Backend Logic:** Robust Apex classes, triggers, and automated test classes ensuring high code coverage.
*   **Modern User Interface:** Built using Lightning Web Components (LWC) and Visualforce pages for dynamic user experiences.
*   **Data Integrity & Security:** Validation rules, formula fields, and granular role-based security (Profiles, Permission Sets, Sharing Rules).
*   **Analytics & Reporting:** Custom reports and interactive dashboards tracking appointment trends, billing metrics, and patient demographics.

---

## 🛠️ Tech Stack

| Area | Technology / Components |
| :--- | :--- |
| **Platform** | Salesforce Developer Edition Org |
| **Data Model** | Custom Objects, Custom Fields, Master-Detail & Lookup Relationships |
| **Automation** | Screen Flows, Record-Triggered Flows, Scheduled Flows, Approval Processes |
| **Backend Logic** | Apex (Classes, Triggers, Test Classes) |
| **User Interface** | Lightning Web Components (LWC), Visualforce, Salesforce Lightning Design System (SLDS) |
| **Analytics** | Salesforce Reports & Dashboards |
| **Tooling & CI/CD** | Salesforce CLI (`sf`), VS Code (Salesforce Extension Pack), Git & GitHub |

---

## 📊 Core Data Model

| Object Name | API Name | Purpose / Description |
| :--- | :--- | :--- |
| **Patient** | `Patient__c` | Stores comprehensive personal and medical history details. |
| **Doctor** | `Doctor__c` | Maintains physician profiles, specializations, and availability. |
| **Appointment** | `Appointment__c` | Junction-style core object linking a Patient to a Doctor for a scheduled visit. |
| **Prescription** | `Prescription__c` | Tracks medicines, dosage instructions, and clinical notes per appointment. |
| **Billing** | `Billing__c` | Manages itemized charges, invoice statuses, and payment tracking. |

---

## 📂 Project Structure

This project follows standard **Salesforce DX (sfdx)** source-driven architecture:

```text
Healthcare_Appointment_Patient_CRM/
│
├── force-app/main/default/
│   ├── objects/              # Custom objects, fields, validation rules
│   ├── classes/              # Apex classes and test classes
│   ├── triggers/             # Apex triggers
│   ├── flows/                # Screen, Record-Triggered, and Scheduled flows
│   ├── approvalProcesses/    # Approval workflows
│   ├── pages/                # Visualforce pages
│   ├── lwc/                  # Lightning Web Components
│   ├── reports/              # Custom reporting folders
│   └── dashboards/           # Analytics dashboards
│
├── docs/screenshots/         # Application UI screenshots
└── sfdx-project.json         # Project configuration
