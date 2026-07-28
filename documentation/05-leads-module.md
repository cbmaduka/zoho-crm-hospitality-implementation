# Leads Module Configuration

## Purpose

The Leads module is used to capture and manage prospective guests before they become customers.

This approach ensures all enquiries are tracked, qualified, and followed through a structured sales process before being converted into Contacts, Accounts, and Deals.

---

# Lead Sources

The following lead sources will be configured:

- Hotel Website
- Phone Enquiry
- Walk-in Guest
- Email
- Facebook
- Instagram
- Travel Agency
- Corporate Referral
- Returning Guest Referral
- Online Travel Agency (OTA)

---

# Information Captured

Each lead should capture:

- Guest Name
- Phone Number
- Email Address
- Lead Source
- Preferred Room Type
- Check-in Date
- Check-out Date
- Number of Guests
- Special Requests
- Assigned Sales Representative

---

# Business Benefits

Using the Leads module enables the hotel to:

- Track all enquiries
- Improve follow-up consistency
- Measure enquiry sources
- Increase booking conversion
- Reduce lost opportunities

---

## Consultant's Notes

The Leads module is intentionally positioned as the entry point into the CRM because hospitality businesses receive enquiries from multiple channels. Qualifying enquiries before converting them into Contacts and Deals helps maintain accurate customer records, reduces duplicate data, and improves sales reporting.

---

# Configuration Completed

## Lead Source

The default Lead Source values were replaced with hospitality-specific enquiry channels to improve reporting and accurately identify where prospective guests originate.

Configured values include:

- Hotel Website
- Phone Enquiry
- Walk-in Guest
- Email
- WhatsApp
- Facebook
- Instagram
- Google Search
- Travel Agency
- Online Travel Agency (OTA)
- Corporate Referral
- Returning Guest Referral
- LinkedIn

---

## Consultant's Notes

Replacing generic sales lead sources with hospitality-specific channels enables management to evaluate marketing effectiveness, identify the most successful booking channels, and allocate resources toward the highest-performing sources of guest enquiries.

---

# Reservation Details Section

A custom section named **Reservation Details** was created to capture information required for hotel reservations.

## Fields Added

| Field | Type |
|--------|------|
| Booking Type | Pick List |
| Check-in Date | Date |
| Check-out Date | Date |
| Number of Guests | Number |
| Room Type | Pick List |
| Number of Rooms | Number |

## Consultant's Notes

Standard CRM fields do not capture reservation-specific information required by the hospitality industry. The Reservation Details section was introduced to organize booking information in a structured format, making it easier for reservations staff to qualify enquiries and prepare quotations.

---

# Guest Preferences

The Guest Preferences section captures service-related information that helps personalize the guest experience.

## Fields Added

| Field | Type |
|--------|------|
| Preferred Contact Method | Pick List |
| Meal Plan | Pick List |
| Airport Pickup Required | Checkbox |
| Loyalty Programme Member | Checkbox |
| Special Requests | Multi-line Text |

## Consultant's Notes

Capturing guest preferences during the enquiry stage enables reservations staff to prepare accurate quotations and deliver a more personalized guest experience while reducing manual follow-up.

---

# Event Details

The Event Details section captures information relating to weddings, conferences, seminars, celebrations, and other functions hosted by LuxeStay Hotels.

## Fields Added

| Field | Type |
|--------|------|
| Event Type | Pick List |
| Event Date | Date |
| Expected Attendees | Number |
| Venue Required | Pick List |
| Catering Required | Checkbox |

## Event Type Values

- Wedding
- Conference
- Seminar
- Birthday
- Anniversary
- Corporate Event
- Other

## Venue Options

- Grand Ballroom
- Conference Hall A
- Conference Hall B
- Garden
- Restaurant
- Private Dining Room

## Consultant's Notes

The Event Details section allows event enquiries to be managed within the same CRM environment as accommodation enquiries. Capturing the event type, date, attendance estimate, venue preference, and catering requirement enables the hotel team to assess capacity, prepare quotations, and coordinate follow-up activities more efficiently.

---

# Internal Reservation Tracking

The Internal Reservation Tracking section supports the hotel team in managing ownership, priority, estimated value, and follow-up activities for each enquiry.

## Fields Added

| Field | Type |
|--------|------|
| Assigned Reservation Officer | User Lookup |
| Reservation Priority | Pick List |
| Estimated Booking Value | Currency |
| Follow-up Date | Date |
| Follow-up Notes | Multi-line Text |

## Reservation Priority Values

- Low
- Medium
- High
- VIP

The default value is **Medium**.

## Consultant's Notes

This section provides internal visibility into who is responsible for each enquiry, which opportunities require urgent attention, and when the next follow-up should occur. The estimated booking value also supports pipeline reporting and helps management prioritize high-value opportunities.

# Layout Rules

## Overview

Layout Rules were configured to dynamically adjust the reservation form based on the selected booking type. This reduces unnecessary data entry, improves user experience, and ensures that staff only see fields relevant to the reservation being processed.

---

## Configured Rules

### Wedding

Condition:
- Booking Type(s) = Wedding

Action:
- Display the **Event Details** section.

---

### Business Travel

Condition:
- Booking Type(s) = Business Travel

Action:
- Display the **Corporate Booking Details** section.

---

### Group Booking

Condition:
- Booking Type(s) = Group Booking

Action:
- Display group reservation fields such as Number of Guests and Number of Rooms.

---

### Long Stay

Condition:
- Booking Type(s) = Long Stay

Action:
- Display long-stay reservation tracking fields.

---

## Business Benefits

- Simplifies data entry
- Reduces user error
- Improves data quality
- Displays only relevant reservation information
- Provides a tailored experience for different reservation scenarios

---

## Consultant's Notes

Dynamic Layout Rules were implemented to improve usability by adapting the reservation form to different booking scenarios. This minimizes unnecessary fields, improves operational efficiency, and helps reservation staff capture only the information required for each type of enquiry.
