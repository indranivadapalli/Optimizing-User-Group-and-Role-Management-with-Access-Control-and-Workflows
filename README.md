ServiceNow Project: Optimizing User, Group, Role, Table, ACL, and Workflow Management

This project introduces a clear framework for defining and organizing users, groups, roles, tables, ACLs, and workflows in ServiceNow, specifically tailored for a small project management team.
Project Overview

The goal of this solution is to address gaps in role assignments, access restrictions, and workflow clarity within project management. It illustrates how a ServiceNow setup can improve accountability, simplify task delegation, and enhance progress monitoring for roles like Project Manager and Team Member.
Features

User setup and management (Project Manager, Team Member)

Group creation for team collaboration

Role-based permissions for controlled access

Custom tables to manage projects and tasks

Assignment of users into groups and roles

Application access control by role

ACL (Access Control List) for data protection

Automated workflows in Flow Designer for task tracking and approvals
Installation & Setup
Prerequisites

Access to a ServiceNow instance

Administrator rights in ServiceNow

Steps

Create Users

Go to: All > Users (System Security)

Add two users: Alice (Project Manager) and Bob (Team Member)

Create Groups

Go to: All > Groups (System Security)

Make a group called Project Team Group and add Alice and Bob

Create Roles

Go to: All > Roles (System Security)

Define new roles: projectmanager, teammember

Set permissions according to each role’s responsibilities

Assign Roles to Users

Open user records and attach the appropriate roles

Create Tables

Build a Project Table and a Task Table

Add fields for name, description, assigned user, status, and comments

Assign Users to Groups

Edit the Project Team Group and confirm Alice and Bob are included

Assign Applications to Roles

Link table applications to the matching roles through Application Navigator

Configure ACLs

Add access control rules for each table

Restrict permissions so only the right roles can edit statuses or comments

Test using impersonation to confirm proper access levels

Design Workflows

Use Flow Designer to build automation:

Trigger: when a Task record is created or updated

Actions: update task status automatically, initiate approval requests

Test Workflow

Modify task records to confirm workflow triggers and approval processes function correctly
Conclusion

This setup delivers structured role definitions, controlled access, secure data handling, and automated workflows that streamline project task management.
Getting Started Clone the repository

git clone https://github.com/your-username/your-repo-name.git

Set up a ServiceNow Developer instance at https://developer.servicenow.com/.

Follow the documentation or wiki provided in this repo for step-by-step setup instructions.

Demo Link

https://drive.google.com/file/d/1HdnR2D2HK088ebHSihHSlopydOv0uTxD/view?usp=sharing

Usage

Project managers can create, assign, and update tasks.

Team members can view and update only their assigned tasks.

Changes to task status and comments are handled securely via ACLs.

Workflow rules automate task status updates and approvals.

Support For further assistance, please refer to ServiceNow official documentation or contact your ServiceNow administrator.
