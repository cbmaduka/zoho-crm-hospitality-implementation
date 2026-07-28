# Workflow Automation

## Overview

Workflow Automation was implemented to streamline reservation management by automatically categorizing wedding enquiries and scheduling timely follow-up activities. The automation reduces manual intervention, improves response time, and ensures reservation staff follow a standardized process when handling wedding bookings.

---

# Workflow Rule

## Rule Name

**Assign Wedding Reservations**

### Module

Leads

### Trigger

- Record Action
- Execute when a Lead record is created.

### Condition

Booking Type(s) = Wedding

---

## Instant Action

### Field Update

Field Updated

- Lead Status

Updated Value

- Contacted

Purpose

Wedding enquiries are automatically marked as **Contacted** immediately after creation, indicating that the reservation team has begun processing the enquiry.

---

## Scheduled Action

### Execution Time

- 1 day after the Lead is created.

### Task Created

**Subject**

- Schedule Meeting

**Status**

- In Progress

**Priority**

- High

**Assigned To**

- Lilian Onyeagba

**Notification**

- Notify assignee enabled.

### Business Purpose

Wedding reservations require early engagement with prospective clients. The automated task ensures that an Events Coordinator schedules an initial consultation with the bride to discuss:

- Wedding date
- Venue requirements
- Expected number of guests
- Accommodation requirements
- Catering preferences
- Decoration requirements
- Payment schedule
- Event logistics

By automatically generating a high-priority follow-up task, the organization ensures that wedding enquiries receive prompt attention and consistent service.

---

## Business Benefits

- Automatically identifies wedding enquiries.
- Eliminates manual follow-up scheduling.
- Ensures every wedding enquiry receives timely attention.
- Standardizes reservation handling procedures.
- Improves response time and customer experience.
- Reduces the risk of missed follow-up activities.

---

## Configuration Summary

| Component | Configuration |
|-----------|---------------|
| Module | Leads |
| Trigger | Lead Created |
| Condition | Booking Type(s) = Wedding |
| Instant Action | Update Lead Status to Contacted |
| Scheduled Action | Create Schedule Meeting Task |
| Delay | 1 Day After Record Creation |
| Task Priority | High |
| Task Status | In Progress |
| Notification | Enabled |

---

## Screenshots

- Workflow Rules Overview
- Wedding Reservation Workflow
- Wedding Field Update Configuration
- Wedding Scheduled Task Configuration

---

## Consultant's Notes

This workflow demonstrates Zoho CRM Workflow Automation by combining conditional logic, field updates, and scheduled tasks within a single business process. The implementation reduces manual effort while ensuring that wedding reservations follow a consistent operational workflow from enquiry through initial consultation.
