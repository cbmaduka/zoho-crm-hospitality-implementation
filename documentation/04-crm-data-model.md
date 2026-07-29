# CRM Data Model

## Overview

The LuxeStay Hotels CRM implementation is designed around a lead-driven reservation process. Guest enquiries enter the CRM through the Leads module, where reservation details are captured, qualified, and managed before conversion.

The data model was designed to support hospitality reservation workflows while maintaining a structured customer lifecycle within Zoho CRM.

---

# Primary Module

## Leads

The Leads module serves as the entry point for all guest enquiries, including accommodation requests, corporate bookings, and event reservations.

It stores reservation information, guest preferences, follow-up activities, and booking qualification details until the enquiry is ready to be converted.

---

# CRM Lifecycle

The reservation process follows the lifecycle below:

**Lead → Contact → Account → Deal**

- **Lead** captures the initial guest enquiry.
- **Contact** represents the confirmed guest.
- **Account** represents an organization for corporate bookings.
- **Deal** represents a confirmed reservation opportunity.

Although this implementation focuses primarily on the Leads module, the data model follows Zoho CRM's standard relationship between these modules.

---

# Integrated CRM Features

The Leads module is integrated with the following CRM components:

- Layout Configuration
- Custom Fields
- Layout Rules
- Validation Rules
- Workflow Automation
- Blueprint
- Reports
- Dashboards
- Knowledge Base

These configurations work together to automate reservation management and improve operational efficiency.

---

# Business Value

This data model provides a structured framework for managing guest enquiries from initial contact through reservation confirmation.

The architecture supports consistent data capture, workflow automation, business reporting, and future scalability as additional CRM modules are implemented.

---

## Screenshots

- Leads Module Overview
- Lead Record
