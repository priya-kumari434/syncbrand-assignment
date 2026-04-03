# Role-Based Dashboard Design

The SyncBrand SaaS platform serves multiple types of users — each with different responsibilities, priorities, and data needs. A role-based dashboard ensures that every user sees only the information most relevant to their role, reducing cognitive overload and improving decision-making speed. Below is a detailed design specification for four primary user roles.

---

## Dashboard Roles Overview

| Role | Primary Goal | Key Modules |
|------|-------------|-------------|
| Admin | Full platform oversight and control | All modules |
| Sales Executive | Manage and convert leads | Leads, Clients, Invoices |
| Designer / Team Member | Deliver project tasks on time | Projects, Tasks, Files |
| Client | Track project progress and manage deliverables | Projects, Files, Invoices |

---

## Dashboard Designs

### Admin

- **Visible Info:**
  - Total leads this month vs. last month (with % change indicator)
  - Revenue overview: total invoiced, paid, and outstanding amounts
  - Active projects count, overdue projects flagged in red
  - Team performance metrics: tasks completed per member, utilization rates
  - Marketing funnel summary: leads → contacted → proposal → won/lost
  - Recent platform activity log (logins, file uploads, status changes)
  - Quick-view notifications: overdue invoices, stalled leads, and missed deadlines

- **Actions:**
  - Add, edit, or deactivate any user account and assign roles
  - Override or reassign leads, projects, and tasks across all team members
  - Generate and export full platform reports (PDF/CSV) for any module
  - Configure platform settings: pipeline stages, invoice templates, access controls
  - View and manage all invoices, approve discounts, and track payment status
  - Set up and modify workflow automation rules

- **Access:**
  - Full access to all modules: Leads, Clients, Projects, Tasks, Files, Invoices, Marketing Analytics
  - User Management panel
  - Platform Settings & Configurations
  - Audit Logs and Activity Reports
  - Billing and Subscription Management

---

### Sales Executive

- **Visible Info:**
  - Personal lead pipeline with stage-wise breakdown (Kanban or list view)
  - Today's follow-up reminders and scheduled calls
  - Lead scoring indicators for prioritizing outreach
  - Win rate and conversion metrics for the current month
  - Recent client interactions and communication history
  - Pending proposals awaiting client response
  - Notifications: new lead assigned, lead moved to negotiation, proposal approved

- **Actions:**
  - Create, update, and move leads through pipeline stages
  - Log call notes, emails, and meeting summaries against each lead
  - Send proposal documents directly from the platform
  - Convert a won lead into a new client and initiate project creation
  - Generate and send invoices for won deals
  - Schedule follow-up tasks and set reminders

- **Access:**
  - Leads module (own leads by default; team leads if manager role is enabled)
  - Clients module (view and edit own clients)
  - Invoices module (create and track own invoices)
  - Files module (upload/download proposal and contract documents)
  - Projects module (read-only view for projects linked to their clients)

---

### Designer / Team Member

- **Visible Info:**
  - Personal task list for today and the upcoming week, sorted by deadline
  - Project progress bars for all active projects they are assigned to
  - Overdue tasks highlighted with urgency indicators
  - File upload/download history for current projects
  - Comments and feedback received from clients or project managers
  - Milestone calendar showing key project deadlines
  - Notifications: new task assigned, deadline approaching, client feedback received

- **Actions:**
  - Update task status: To Do → In Progress → Review → Completed
  - Upload deliverable files and tag them to specific project milestones
  - Leave comments or questions on tasks and project threads
  - Request deadline extensions with a justification note
  - View and download project briefs, brand guidelines, and reference files
  - Log time spent on tasks (if time tracking is enabled)

- **Access:**
  - Projects module (projects they are assigned to only)
  - Tasks module (own tasks; team tasks if team lead role)
  - Files module (upload/download within assigned projects)
  - No access to: Leads, Clients, Invoices, Marketing Analytics, or User Management

---

### Client

- **Visible Info:**
  - Active project(s) status with current milestone and overall completion percentage
  - Timeline view of project phases and upcoming deliverable dates
  - Files shared by the SyncBrand team, organized by project phase
  - Invoice history: paid, pending, and upcoming payment schedules
  - Feedback threads and communication history with the project team
  - Notifications: new file uploaded, milestone completed, invoice issued, message received

- **Actions:**
  - View and download deliverable files uploaded by the team
  - Approve or request revisions on specific deliverables with comments
  - Upload reference files, brand assets, or feedback documents
  - View, download, and pay invoices through an integrated payment gateway
  - Send messages to the project coordinator within the platform
  - Update their own profile and company information

- **Access:**
  - Projects module (their project(s) only — read-only on timelines)
  - Files module (files linked to their project only)
  - Invoices module (their invoices only — view and pay)
  - Messaging/Communication thread (linked to their project)
  - No access to: Leads, other Clients' data, Team Tasks, Marketing Analytics, or Admin settings

---

## Design Principles

1. **Minimal Cognitive Load** — Each dashboard surfaces only the data that is actionable for that role. Irrelevant modules are hidden, not just disabled.
2. **Glanceable KPIs** — Key metrics appear as visual cards at the top of each dashboard so users get their most important information at a glance without scrolling.
3. **Action-Centric Layout** — Primary actions (e.g., "Add Lead," "Upload File," "Mark Complete") are one click away from the dashboard without navigating to a separate module.
4. **Notification Center** — A unified in-app notification panel keeps each user informed of events relevant to their role, reducing dependency on email updates.
5. **Responsive Design** — All dashboards are optimized for both desktop and mobile, allowing sales reps and clients to use the platform on the go.

---

*Prepared for SyncBrand Media Pvt. Ltd.*
