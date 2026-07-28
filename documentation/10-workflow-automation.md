# Workflow Automation

## Overview

Workflow automation was implemented in the Zoho CRM Hospitality Leads module to automate the handling of wedding reservation enquiries.

The automation ensures that every wedding enquiry receives immediate attention, is prioritised appropriately, and generates a follow-up task without requiring manual intervention.

---

## Workflow Name

**Assign Wedding Reservations**

---

## Module

Leads

---

## Trigger

- Execute On: Record Creation
- Condition:
  - Booking Type(s) = Wedding

---

## Business Process

When a new wedding reservation enquiry is created, Zoho CRM automatically classifies the enquiry as a priority reservation by updating the Lead Status to **Contacted**.

One hour after the enquiry is created, the system generates a high-priority task assigned to the reservation coordinator to contact the bride and schedule an initial consultation.

The task is due one day from the record creation date, ensuring timely follow-up while allowing the reservations team adequate time to prepare.

---

## Instant Actions

### Field Update

| Field | Value |
|-------|-------|
| Lead Status | Contacted |

Purpose:

- Immediately identifies the enquiry as being actively handled.
- Removes the need for manual status updates.
- Ensures reservation staff can quickly distinguish active enquiries from new submissions.

---

## Scheduled Actions

### Task Creation

| Property | Value |
|----------|-------|
| Subject | Schedule Meeting |
| Priority | High |
| Status | In Progress |
| Assigned To | Reservation Coordinator |
| Execution Time | 1 Hour After Record Creation |
| Due Date | 1 Day After Record Creation |

Purpose:

- Reminds the reservations team to promptly engage with the prospective client.
- Encourages timely consultation and relationship building.
- Reduces the likelihood of missed or delayed follow-up on high-value wedding enquiries.

---

## Business Value

This workflow automation provides several operational benefits:

- Eliminates repetitive manual task creation.
- Standardises the handling of wedding reservations.
- Improves response times for premium bookings.
- Ensures accountability through automated task assignment.
- Enhances customer experience by guaranteeing timely follow-up.

---

## Screenshots

- `workflow-rule-overview.png`
- `assign-wedding-reservations-workflow.png`
- `wedding-booking-field-update.png`
- `schedule-meeting-task.png`
