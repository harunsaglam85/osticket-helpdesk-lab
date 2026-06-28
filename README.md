# osTicket Helpdesk Lab

A fully functional IT helpdesk system I deployed from scratch on a Linux server in the cloud. This project demonstrates real-world skills used by IT support professionals every day — setting up servers, managing databases, and handling support tickets.

**Live URL:** http://5.78.236.153

---

## What is osTicket?

osTicket is an open-source helpdesk ticketing system used by IT departments worldwide. When a user has a technical problem, they submit a ticket. The IT team receives it, investigates, responds, and closes it when resolved. This is the backbone of every IT support operation.

---

## Environment

| Component | Details |
|-----------|---------|
| Server | Hetzner VPS (Ubuntu 22.04) |
| Web Server | Apache2 |
| Database | MySQL |
| Application | osTicket v1.18.1 |
| Live URL | http://5.78.236.153 |

---

## What I Built

- Provisioned a cloud Linux server (Ubuntu 22.04) on Hetzner
- Installed and configured a full LAMP stack (Linux, Apache, MySQL, PHP) from scratch via command line
- Created a dedicated MySQL database and user with proper permissions
- Configured Apache virtual host with URL rewriting (mod_rewrite)
- Downloaded, extracted, and installed osTicket v1.18.1 via the web installer
- Secured the installation by removing the setup directory and locking the config file
- Demonstrated a complete ticket lifecycle from submission to resolution

---

## Walkthrough

### Step 1 — Installer Prerequisites Check
![Prerequisites](screenshots/01-installer-prerequisites.png)

After navigating to the server IP in the browser, the osTicket installer runs a prerequisites check. Every required PHP extension shows a green checkmark — confirming the server is properly configured to run the application. This is the result of manually installing each PHP module via the command line.

---

### Step 2 — Installation Complete
![Installation Complete](screenshots/02-installation-complete.png)

After filling in the helpdesk name, admin account details, and database credentials, osTicket confirms a successful installation. The page provides links to the admin panel and user portal, and instructs to remove the setup directory for security — which I completed immediately.

---

### Step 3 — Admin Ticket Queue
![Admin Queue](screenshots/03-admin-ticket-queue.png)

This is the admin dashboard where IT staff manage incoming tickets. Each ticket shows the ticket number, subject, timestamp, submitter, and priority. From here, tickets can be assigned to staff, escalated, or resolved. This view mirrors what a real IT helpdesk analyst sees every day.

---

### Step 4 — Ticket Thread with Admin Response
![Ticket Thread](screenshots/04-ticket-thread-response.png)

Inside a ticket, the full conversation thread is visible. The user submitted a report about their computer not connecting to the network. The admin (me) responded with a reply. The system tracks every message, timestamp, assignment, SLA plan, and due date — creating a full audit trail.

---

### Step 5 — Ticket Submitted Successfully
![Ticket Submitted](screenshots/05-ticket-submitted.png)

This is what the end user sees after submitting a support request through the user portal. The system confirms the ticket was created and notifies the user that a representative will follow up. Clean and professional — exactly what users expect from an IT support system.

---

### Step 6 — User Portal
![User Portal](screenshots/06-user-portal.png)

The public-facing user portal where anyone can submit a support ticket or check the status of an existing one. This is the front door of the helpdesk. Built and hosted entirely on my own Linux server — no third-party hosting involved.

---

### Step 7 — Ticket Detail View
![Ticket Detail](screenshots/07-ticket-detail.png)

A detailed view of an open ticket showing all metadata: status, priority, department, SLA plan, due date, assigned agent, and the full message thread. This level of detail is what allows IT teams to track, prioritize, and resolve issues efficiently.

---

## Skills Demonstrated

- Linux server administration (Ubuntu 22.04)
- Apache2 web server configuration and virtual hosting
- MySQL database creation and user permissions
- PHP environment setup and module management
- IT helpdesk administration and ticket lifecycle management
- Security hardening post-installation
- Technical documentation and SOP adherence
