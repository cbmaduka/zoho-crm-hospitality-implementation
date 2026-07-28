# Blueprint Configuration

## Overview

A Blueprint was created to standardize the initial handling of hotel booking enquiries in the Hospitality Lead Layout.

The Blueprint ensures that every new booking enquiry follows a defined process before progressing to the next reservation stage. This helps maintain operational consistency and ensures reservation enquiries are handled promptly.

---

## Blueprint Configuration

| Setting | Value |
|---------|-------|
| Module | Leads |
| Layout | Hospitality |
| Blueprint Name | Hotel Booking |
| Entry Criteria | Lead Status = New Enquiry |

---

## Initial Process

Every record entering the Blueprint begins with the **New Enquiry** status.

The first transition, **Contact Guest**, represents the reservation team's first interaction with the customer.

During this transition, reservation staff can review booking information, capture any required details, and update the enquiry before moving it to the **Contacted** stage.

---

## Transition

**Transition Name**

Contact Guest

**From**

New Enquiry

**To**

Contacted

**Purpose**

- Standardize the initial response process
- Ensure every enquiry receives human follow-up
- Prevent enquiries from remaining unattended
- Improve reservation response consistency

---

## Transition Configuration

The transition includes configurable sections for:

- Before Transition
- During Transition
- After Transition

These allow administrators to:

- Display mandatory fields
- Request additional booking information
- Trigger follow-up actions
- Send notifications
- Execute field updates
- Create records
- Call webhooks
- Execute custom actions

---

## Business Value

Implementing a Blueprint introduces process governance into the reservation workflow by ensuring each enquiry progresses through predefined stages rather than relying on manual updates.

This minimizes missed enquiries, improves response times, and provides better visibility into the reservation lifecycle.
