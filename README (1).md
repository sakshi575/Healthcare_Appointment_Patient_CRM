# Healthcare Appointment & Patient CRM

`Healthcare_Appointment_Patient_CRM`

An end-to-end **Salesforce CRM** for managing patients, doctors, appointments, prescriptions and billing in a healthcare setting. Built on the Salesforce Platform with custom objects, Flow automation, Apex, Visualforce, Lightning Web Components, and reports and dashboards.

Final-year B.Tech project by **Sakshi Singh**.

## Features

- **Patient, doctor and appointment management** in one connected data model
- **Prescription and billing tracking** linked to each appointment
- **Flow automation:** Screen Flow for guided data entry, Record-Triggered Flow for instant updates, Scheduled Flow for recurring tasks
- **Approval Process** for records that need sign-off
- **Apex class and trigger** for custom business logic, with a **test class** for code coverage
- **Visualforce page** and two **Lightning Web Components** for the user interface
- **Validation Rules and Formula Fields** to keep data clean
- **Role-based security** through users, profiles and permissions
- **Reports and a dashboard** for appointment and patient insights

## Build Phases

The project was built in 20 phases, from org setup to final testing.

| Phase | Step |
| --- | --- |
| 1 | Create Salesforce Org |
| 2 | Create Objects |
| 3 | Create Fields |
| 4 | Create Relationships |
| 5 | Create Sample Data |
| 6 | Validation Rules & Formula Fields |
| 7 | Create Users & Security |
| 8 | Screen Flow |
| 9 | Record-Triggered Flow |
| 10 | Scheduled Flow |
| 11 | Approval Process |
| 12 | Apex Class |
| 13 | Apex Trigger |
| 14 | Test Class |
| 15 | Visualforce |
| 16 | LWC #1 |
| 17 | LWC #2 |
| 18 | Reports |
| 19 | Dashboard |
| 20 | Testing & Presentation |

## Tech Stack

| Area | Technology |
| --- | --- |
| Platform | Salesforce (Developer Edition org) |
| Data model | Custom objects, fields, relationships |
| Automation | Screen Flow, Record-Triggered Flow, Scheduled Flow, Approval Process |
| Backend logic | Apex (class, trigger, test class) |
| UI | Visualforce, Lightning Web Components (LWC) |
| Analytics | Reports and Dashboards |
| Tooling | Salesforce CLI, VS Code with Salesforce Extension Pack, Git |

## Data Model

| Object | Purpose |
| --- | --- |
| Patient | Stores patient details |
| Doctor | Stores doctor details |
| Appointment | Links a patient with a doctor for a visit |
| Prescription | Medicines prescribed during an appointment |
| Billing | Charges and payment status for an appointment |

## Project Structure

This is a Salesforce DX project.

```
force-app/main/default/
  objects/              Custom objects, fields, validation rules
  classes/              Apex classes and test classes
  triggers/             Apex triggers
  flows/                Screen, Record-Triggered and Scheduled flows
  approvalProcesses/    Approval processes
  pages/                Visualforce pages
  lwc/                  Lightning Web Components
  reports/              Reports
  dashboards/           Dashboards
docs/screenshots/       Screenshots used in this README
sfdx-project.json       Project configuration
```

## Getting Started

### Prerequisites

- [Salesforce CLI](https://developer.salesforce.com/tools/salesforcecli)
- [VS Code](https://code.visualstudio.com/) with the [Salesforce Extension Pack](https://developer.salesforce.com/tools/vscode/)
- A free [Developer Edition org](https://developer.salesforce.com/signup)

### Deploy to your own org

```bash
# 1. Clone the repository
git clone https://github.com/sakshi575/Healthcare_Appointment_Patient_CRM.git
cd Healthcare_Appointment_Patient_CRM

# 2. Log in to your org
sf org login web --alias healthcare-crm

# 3. Deploy the metadata
sf project deploy start --source-dir force-app --target-org healthcare-crm

# 4. Run the Apex tests
sf apex run test --target-org healthcare-crm --result-format human --wait 10

# 5. Open the org
sf org open --target-org healthcare-crm
```

## Author

**Sakshi Singh**, final-year B.Tech Computer Science and Engineering (Data Science)

[GitHub](https://github.com/sakshi575) | [LinkedIn](https://linkedin.com/in/sakshisingh71)
