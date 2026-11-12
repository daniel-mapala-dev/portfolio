# CEDEP Integrated Management System (CIMS)

**Client:** Centre for the Development of People (CEDEP), Lilongwe, Malawi
**Year:** 2025
**Role:** Architect and lead developer
**Status:** In production

---

## The problem

CEDEP's health, research, advocacy, and administrative functions each
maintained separate records. This produced data silos, duplicated entry,
and no single trusted source for organisational reporting.

## The solution

An enterprise web platform integrating four functional domains into a
unified data model:

- **Health** — programme delivery and participant records
- **Research** — study data, participant tracking, and reporting
- **Advocacy** — case and activity tracking
- **Administration** — staff, assets, and operational records

Shared reference data (people, locations, projects) sits at the centre of
the model, so a single record serves all four domains.

## My role

Architect and lead developer. Requirements gathering across departments,
data model design, application development, integration design, testing,
deployment, and staff training.

## Architecture

| Layer | Technology |
| :--- | :--- |
| Application | Laravel (PHP) |
| Database | MySQL |
| Frontend | Blade, JavaScript |
| Integration | REST APIs between modules and external partner systems |
| Access control | Role-based, domain-scoped |

## Design decisions

**Shared reference data at the centre.** Rather than four systems
exchanging data, one schema holds shared entities and each domain extends
them. This eliminated the reconciliation problems that separate systems
would have created.

**API-first integration.** Partner systems connect through REST APIs
rather than direct database access, which preserves security boundaries
and allows partner changes without affecting the core schema.

**Domain-scoped permissions.** A research officer sees research data and
shared reference data, but not advocacy case records. Permissions are
scoped by domain rather than by module.

## What this demonstrates

Enterprise information architecture · unified data modelling across
domains · REST API design · role-scoped access control · integration
of legacy departmental systems.

## Code availability

Source code is private under client agreement. A technical walkthrough
can be provided on request.
