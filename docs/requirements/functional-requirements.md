# Functional Requirements
## Real Estate Agency Management System

---

## 1. Lead Management

The following requirements come from Sara's need to respond to new leads instantly and Marco's need to stay on top of clients who have gone quiet.

The system shall notify an agent in real time when a new lead is assigned to them, including the client's name, contact number, and inquiry summary.

The system shall automatically create a client profile when a new lead is submitted through the agency website, capturing all details from the inquiry form.

The system shall allow agents to log client preferences including budget range, preferred location, property type, and number of bedrooms.

The system shall flag any client who has had no logged interaction for more than a configurable number of days and notify the responsible agent.

The system shall allow agents to set a follow-up reminder on any client with a due date and a note describing the reason for the follow-up.

The system shall send the agent a notification on the day a follow-up reminder is due, including the client's name and the note left at the time of setting the reminder.

The system shall display overdue follow-up reminders prominently on the agent's dashboard so that they cannot be missed.

---

## 2. Client Profile & Interaction History

The following requirements come from Sara's need to have full context on every client before a call or meeting, without relying on paper notes.

The system shall maintain a full chronological interaction history for every client, including calls, emails, viewings, and notes.

The system shall allow agents to add a new interaction log entry to any client profile, including the type of contact, date, and a summary note.

The system shall display client preferences at the top of the client profile so they are visible immediately when the profile is opened.

The system shall allow agents to update or correct client preferences at any time.

---

## 3. Property Management

The following requirements come from Sara's need to keep listings accurate from any device and Marco's need to be alerted when a property has stalled.

The system shall allow agents to create a new property listing with fields for address, price, size, type, description, and current status.

The system shall allow agents to edit any field on an existing property listing at any time, with changes reflected immediately across the system.

The system shall allow agents to upload multiple photos and supporting documents to any property listing.

The system shall allow agents to archive a property listing when it is no longer available, removing it from active search results without deleting it permanently.

The system shall allow agents to search and filter properties by price range, location, property type, number of bedrooms, and availability status.

The system shall automatically suggest matching properties to an agent based on a client's saved preferences.

The system shall notify the responsible agent when a property has had no viewings or activity for more than a configurable number of days.

The system shall display all stale properties on the manager dashboard, sorted by how long they have been inactive.

---

## 4. Appointment & Viewing Scheduler

The following requirements come from Sara's need to avoid double bookings and James's need to receive reminders so he does not miss viewings.

The system shall allow agents to create a viewing appointment linked to a specific property and client.

The system shall check for scheduling conflicts before confirming a new viewing appointment and prevent the booking if a conflict exists.

The system shall display all of an agent's upcoming appointments in a personal calendar view.

The system shall send the client an automatic confirmation when a viewing is booked, including the property address, date, time, and agent contact details.

The system shall send the client an automatic reminder 24 hours before their scheduled viewing.

The system shall send the agent an automatic reminder 1 hour before a scheduled viewing.

The system shall allow agents to cancel or reschedule a viewing from within the system and notify the client automatically when this happens.

The system shall prompt the agent to log client feedback immediately after a viewing is marked as completed.

The system shall allow feedback to be submitted from a mobile device using a simple rating and notes field.

The system shall save viewing feedback to the client's profile and link it to the property that was viewed.

---

## 5. Offer & Negotiation Tracking

The following requirements come from Sara's need to track every offer clearly and James's need to always know the status of his purchase.

The system shall allow agents to log a new offer with the client name, property, offered price, and date.

The system shall display the current status of every offer using clear status labels: Submitted, Counter Offered, Accepted, Rejected, or Withdrawn.

The system shall maintain a full negotiation trail showing every offer and counter offer in chronological order, visible to the agent and manager.

The system shall notify the agency manager when a new offer is submitted and requires their awareness before proceeding.

The system shall allow the manager to approve or reject a deal before the contract stage is reached, with the option to add a written comment.

The system shall notify the agent immediately when the manager approves or rejects a deal.

The system shall notify the client automatically within 5 minutes of their offer status changing, clearly stating the new status and any next steps.

---

## 6. Contract & Document Management

The following requirements come from Sara's need to store documents securely in one place and Lisa's need to ensure nothing is altered without a trace.

The system shall allow agents to upload documents and attach them to a deal, client, or property record.

The system shall allow authorised users to search for documents by name, date, and associated record.

The system shall restrict document access based on user role so that only authorised users can view sensitive files.

The system shall never permanently delete a document — all removed documents must be archived and remain retrievable by an administrator.

The system shall automatically update the property status to Sold when a deal is marked as closed.

The system shall log every document upload and access event in the audit trail, including who accessed it and when.

---

## 7. Commission & Financial Tracking

The following requirements come from Sara's need to trust her commission figure without manual calculation.

The system shall automatically calculate an agent's commission when a deal is marked as closed, based on the final agreed sale price and the agent's configured commission rate.

The system shall display each agent's commission earnings broken down by individual deal on their personal dashboard.

The system shall allow administrators to configure a commission rate per agent or per deal type.

---

## 8. Agent Dashboard

The following requirements come from Sara and Marco's need to have a clear daily overview without having to search for information.

The system shall provide each agent with a personal dashboard showing active leads, upcoming viewings, overdue follow-up reminders, pending deal actions, and progress toward their monthly target.

The system shall auto-generate a daily task list for each agent based on due reminders, upcoming viewings, and open deal actions.

The system shall be fully functional on mobile devices so that agents can use it while on-site at a property or in a client meeting.

The system shall allow agents to log interactions, update client records, and complete tasks from a mobile device.

---

## 9. Manager Dashboard & Reporting

The following requirements come from Diana's need for visibility over her team and the ability to act before problems become too serious.

The system shall provide a manager dashboard showing each agent's performance including leads contacted, viewings completed, deals closed, and revenue generated.

The system shall allow the manager dashboard to be filtered by time period including this week, this month, and a custom date range.

The system shall visually highlight any agent who is significantly below their monthly target so that Diana can identify who needs support at a glance.

The system shall allow managers to set or update a monthly sales target for any individual agent at any time.

The system shall display the target and current progress for every agent on the manager dashboard side by side.

The system shall allow managers to reassign a lead or property from one agent to another directly from the dashboard.

The system shall allow managers to generate a monthly revenue report including total revenue, number of deals closed, and top performing agents.

The system shall allow revenue reports to be exported as a PDF or CSV file.

---

## 10. User Management & Administration

The following requirements come from Lisa's need to control access efficiently and maintain accountability across the system.

The system shall allow administrators to create a new user account with a name, email address, and assigned role.

The system shall automatically send a welcome email with login credentials to a new user the moment their account is created.

The system shall allow administrators to edit or deactivate any user account at any time.

The system shall immediately revoke all system access when a user account is deactivated, with no grace period.

The system shall enforce role-based access control with distinct permission levels for Administrator, Manager, Agent, and Client roles.

The system shall record every action taken in the system in a permanent audit log, including the user who performed it, the action type, the record affected, and the timestamp.

The system shall allow administrators to search and filter the audit log by user, date range, and action type.

The system shall never allow audit log entries to be edited or deleted by any user including administrators.