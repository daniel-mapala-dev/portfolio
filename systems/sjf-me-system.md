# SJF Institutional M&E and Project Tracking System

**Client:** Social Justice Foundation (SJF), Blantyre, Malawi
**Year:** 2026
**Role:** Lead developer and architect
**Status:** Delivered and in production

---

## The problem

SJF managed strategic plan tracking, project results, beneficiary data,
and emergency fund case management across spreadsheets and paper records.
This created duplication, inconsistent reporting, no audit trail, and
significant time spent compiling reports manually.

## The solution

A 12-module web platform covering:

- Strategic Plan management
- Project and activity tracking
- Results frameworks
- Indicator tracking
- Beneficiary and reach data
- Emergency Fund case management (Annexes 1–9)
- Data quality controls
- Role-based access control (RBAC)
- Audit trails
- Automated reporting
- Notification rules with SLA alerts
- Administrative configuration

## My role

Sole architect and developer. I gathered requirements directly with the
CEO and programme staff, designed the data model and system
architecture, developed the application, conducted testing and user
acceptance, deployed to production, and trained staff.

## Architecture

| Layer | Technology |
| :--- | :--- |
| Application | Laravel (PHP) |
| Database | MySQL (relational, normalised) |
| Frontend | Blade templating, JavaScript |
| Access control | Role-based, per-module permissions |
| Audit | Logging on all data-changing operations |

## Design decisions

**Relational model over document storage.** The reporting requirements
depend on consistent aggregation across indicators, projects, and time
periods. A normalised relational model with foreign key integrity was
the right fit.

**RBAC at module and action level.** Programme staff, finance staff, and
senior management need different views of the same data. Permissions are
enforced at both module and action level rather than by page.

**Audit trails on all mutations.** Case management data on vulnerable
beneficiaries requires accountability. Every create, update, and delete
is logged with user, timestamp, and changed fields.

**SLA notifications.** Indicator reporting deadlines are tracked, and
notification rules alert responsible officers before a deadline is
missed.

## What this demonstrates

Multi-module system design · relational data modelling · RBAC
implementation · audit trail design · automated reporting · notification
and SLA logic · end-to-end delivery from requirements to production.

## Code availability

Source code is private under client agreement. A technical walkthrough
can be provided on request.
