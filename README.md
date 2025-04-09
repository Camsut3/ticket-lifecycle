<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to create, work, and resolves tickets within osTicket](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

<h2>Lifecycle Stages</h2>
# osTicket Lifecycle Examples

This document demonstrates **real-world lifecycle examples** for support tickets in osTicket. Each example walks through the journey of a ticket from creation to resolution, showcasing how departments, help topics, agents, and automations interact.

---

## 🎟️ Example 1: Basic IT Support Request

**Scenario**: A user submits a request for a password reset.

- **Help Topic**: Account Support → Password Reset
- **Department**: IT Support
- **Auto-assign**: Yes, based on topic
- **SLA Plan**: 1 Hour First Response

### Lifecycle:
1. User submits ticket via web form.
2. Ticket is auto-assigned to "IT Support" department.
3. Agent receives notification and takes ownership.
4. Agent resets the password and updates ticket.
5. User is notified via email.
6. Ticket is marked "Resolved."
7. After 3 days of inactivity, ticket is automatically closed.

---

## 📦 Example 2: Customer Service – Order Inquiry

**Scenario**: A customer wants to check the status of an order.

- **Help Topic**: Orders → Shipping Status
- **Department**: Customer Service
- **Auto-responder**: Enabled
- **SLA Plan**: 4 Hours Response

### Lifecycle:
1. User emails `support@yourdomain.com`.
2. osTicket pulls in the message and creates a new ticket.
3. Ticket routed to "Customer Service."
4. Auto-response confirms receipt.
5. Agent replies with shipping details.
6. User replies back with additional questions.
7. Agent updates ticket until resolution.
8. Ticket marked "Resolved," then closed after 72 hours of no reply.

---

## 🧾 Example 3: Billing Dispute Ticket

**Scenario**: A user reports a double charge on their invoice.

- **Help Topic**: Billing → Disputes
- **Department**: Finance
- **Priority**: High
- **SLA Plan**: 24 Hours

### Lifecycle:
1. Ticket is created via web or email.
2. Routed to "Finance" department.
3. Finance agent tags ticket as "Urgent."
4. Investigates billing system.
5. Contacts customer with results.
6. Coordinates refund or adjustment.
7. User confirms issue resolved.
8. Ticket is closed.

---

## ⚙️ Example 4: Internal IT Equipment Request

**Scenario**: An employee requests a new monitor.

- **Help Topic**: Internal Request → Equipment
- **Form Fields**: Equipment type, justification
- **Department**: IT Procurement
- **Custom Fields**: Yes (dropdowns, text fields)

### Lifecycle:
1. Employee submits ticket with custom form.
2. Supervisor is auto-notified for approval.
3. Once approved, IT Procurement is notified.
4. Agent assigns task to technician.
5. Technician delivers equipment.
6. Employee confirms receipt.
7. Ticket marked closed.

---

## 🔄 Example 5: Escalated Technical Issue

**Scenario**: A user has a persistent issue with software crashing.

- **Help Topic**: Software Support → App Crashes
- **Department**: Tier 1 Support → Escalation to Tier 2
- **SLA Plan**: 8 Hours Resolution
- **Tasks/Sub-Tickets**: Enabled

### Lifecycle:
1. Ticket created and handled by Tier 1.
2. Tier 1 agent unable to solve and flags as "Needs Escalation."
3. Supervisor re-assigns to Tier 2 Support.
4. Tier 2 agent creates sub-ticket to log testing steps.
5. Issue is fixed and user is updated.
6. Supervisor marks main ticket as resolved.

---

## 📌 Final Notes

These examples can be tailored for any organization’s workflow. You can enhance automation with:

- SLA breach alerts
- Auto-assignments based on Help Topics
- Canned responses
- Custom forms and fields
- Ticket filters
